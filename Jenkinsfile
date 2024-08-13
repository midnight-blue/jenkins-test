pipeline {
    agent none
    stages {
     stage('Initialize'){
               steps {
                script {
                       def dockerHome = tool 'docker'
                       env.PATH = "${dockerHome}/bin:${env.PATH}"
                   }
               }

        }

        stage('Docker Build') {
          agent any
          steps {
            sh 'docker build -t openid:latest .'
          }
        }
    }
}
