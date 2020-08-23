pipeline {
    agent any

    stages {
        stage('Build Discovery Service') {
            steps {
                echo 'Building Discovery Service...'
				bat 'cd ./discovery-service/ && mvn clean install'
            }
        }
        stage('Build API Gateway') {
            steps {
                echo 'Building API Gateway...'
				bat 'cd ./api-gateway/ && mvn clean install'
            }
        }
		stage('Build Car Service') {
            steps {
                echo 'Building Car Service...'
				bat 'cd ./car-service/ && mvn clean install'
            }
        }
        stage('Testing Discovery Service') {
            steps {
                echo 'Testing Discovery Service...'
				bat 'cd ./discovery-service/ && mvn clean test'
            }
        }
        stage('Testing API Gateway') {
            steps {
                echo 'Testing API Gateway...'
				bat 'cd ./api-gateway/ && mvn clean test'
            }
        }
		stage('Testing Car Service') {
            steps {
                echo 'Testing Car Service...'
				bat 'cd ./car-service/ && mvn clean test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
            }
        }
    }
}