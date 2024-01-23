pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        script {
          docker.image('node:16-buster-slim').inside {
            sh 'npm install'
          }
        }
      }
    }
  }
}