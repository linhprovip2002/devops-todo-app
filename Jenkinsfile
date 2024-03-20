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

    stage('Open Image') {
      steps {
        // Replace 'image.jpg' with the name of your image file
        sh 'xdg-open aaa.jpg 
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
