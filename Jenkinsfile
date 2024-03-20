pipeline {
  agent {
    docker {
      image 'node:lts-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Test') {
      steps {
        echo 'hello'
      }
    }

    stage('Install dependency') {
      steps {
        sh 'npm install'
      }
    }

    stage('Run') {
      steps {
        sh 'npm start'
      }
    }

  }
}