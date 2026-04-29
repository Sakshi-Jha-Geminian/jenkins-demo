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
                sh 'node app.js'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test'
            }
        }

        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
    }
}
