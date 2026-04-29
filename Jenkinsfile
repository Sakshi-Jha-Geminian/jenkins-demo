pipeline {
    agent any

    tools {
        nodejs 'NodeJS'
    }

    stages {
        stage('Check Node') {
            steps {
                bat 'node -v'
                bat 'npm -v'
            }
        }

        stage('Run Script') {
            steps {
                bat 'node app.js'
            }
        }

        stage('Test') {
            steps {
                bat 'npm test'
            }
        }

        stage('Build') {
            steps {
                bat 'npm run build'
            }
        }
    }
}
