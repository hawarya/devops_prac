pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/hawarya/devops_prac.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean compile'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
