pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/pateldev11/DEVPATEL-LAB2'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
    }
}