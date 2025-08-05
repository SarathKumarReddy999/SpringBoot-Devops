// This is our first Declarative Jenkins Pipeline
pipeline {
    agent any
    stages {
        stage('Date') {
            steps {
                bat 'date /t' // Example for Windows
            }
        }
        stage('build') {
            steps {
                echo 'Building the spring boot project from git'
            }
        }
        stage('test') {
            steps {
                echo 'Test cases are running and completed from git'
            }
        }
    }
    post {
        always {
            echo 'Pipeline finished, check the console output!'
        }
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed! Review the logs.'
        }
    }
}
