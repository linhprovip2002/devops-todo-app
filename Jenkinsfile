pipeline {
    agent {
        docker {
            image 'node:lts-alpine'
            ports {
                // Expose the port from the container to the host
                port '3000:3000'
            }
        }
    }
    stages {
        stage('Build') {
            steps {
                // Install dependencies
                sh 'npm install'
            }
        }
        stage('Run') {
            steps {
                // Start your Node.js application
                sh 'npm start'
            }
        }
    }
}
