pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Install') {
            steps {
                bat 'npm install'
            }
        }

        stage('Test') {
            steps {
                bat 'npm test'
            }
        }

        stage('CD Trigger') {
            steps {
                echo 'CI Successful - Deployment will be handled by Render'
            }
        }
    }
}
