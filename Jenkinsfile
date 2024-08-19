pipeline{
    stages{
        stage("checkout code stage"){
            steps{
                git url:'https://github.com/Priti407/jenkinsRepo1.git',branch:'main'

           }   
        }   
        stage("Build docker image"){
            steps{
                sh 'docker build -t myimage .'
            }
        }
        stage("create container"){
            steps{
                sh 'docker run -d -p 8501:8501 myimage'
            }
        }

    }
      
}