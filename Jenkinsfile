pipeline {
    agent {
        docker { image 'node:20.11.1-alpine3.19' }
    }
    // set up environment
    environment {
        HOME = '.'
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
        // install application stage
        stage('Install_APP') {
            steps {
                sh 'npm install'
            }
        }
    }
}