pipeline {
    agent {
        docker { image 'node:14' }
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

         // Package application stage
        stage('Pack_APP') {
            steps {
                sh 'npm pack'
            }
        }
    }
}