pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3800:3800'
        }
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
  }
  environment {
    CI = 'true'
  }
}