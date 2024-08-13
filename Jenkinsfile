pipeline {
    agent none
    stages {
        tools {
            docker 'latest'
        }

        stage('Docker Build') {
          agent any
          steps {
            sh 'docker build -t openid:latest .'
          }
        }
    }
}
