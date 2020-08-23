pipeline {
    agent any

    stages {
        stage('Build Discovery Service') {
            steps {
                echo 'Building Discovery Service...'
            }
        }
        stage('Build API Gateway') {
            steps {
                echo 'Building API Gateway...'
            }
        }
		stage('Build Car Service') {
            steps {
                echo 'Building Car Service...'
            }
        }
        stage('Testing Discovery Service') {
            steps {
                echo 'Testing Project Manager Frontend...'    
            }
        }
        stage('Testing API Gateway') {
            steps {
                echo 'Testing API Gateway...'
            }
        }
		stage('Testing Car Service') {
            steps {
                echo 'Testing Car Service...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
            }
        }
    }
}