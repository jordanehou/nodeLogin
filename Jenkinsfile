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
                //sh 'npm install'

                 git branch: 'main', url: 'https://github.com/your/repo.git'

                // Install dependencies and build the Node.js app
                sh 'npm install'
                sh 'npm run build'
            }
        }
    }
}