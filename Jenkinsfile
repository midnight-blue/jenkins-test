pipeline {
    stages {
        stage('Docker Build') {
          agent any
          steps {
            sh 'docker build -t openid:latest .'
         }
    }
}
