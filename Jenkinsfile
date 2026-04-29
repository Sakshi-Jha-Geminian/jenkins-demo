pipeline {
    agent any

    stages {
        stage('Print Hello') {
            steps {
                echo 'Hello, Jenkins!'
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
