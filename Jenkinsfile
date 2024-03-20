pipeline {
  agent any
  
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
        
        sh 'ls -la'
        echo 'Finish'
      }
    }
  }
}
