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
        script {
          try {
            sh 'npm install'
          } catch (Exception e) {
            echo 'npm is not found or npm install failed'
            error('Stopping the build due to npm installation failure.')
          }
        }
      }
    }

    stage('Open todo.ejs in Views Folder') {
      steps {
        dir('views') {
          sh 'xdg-open todo.ejs || open todo.ejs'
        }
      }
    }

    stage('Run') {
      steps {
        echo 'Finish'
      }
    }
  }
}
