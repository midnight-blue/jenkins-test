pipeline {
    agent none
    tools {
        dockerTool 'latest'
    }


    stages {
        stage('Docker Build') {
          agent any
          steps {
            sh 'docker build -t openid:latest .'
          }
        }
    }
}
