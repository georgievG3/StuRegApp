pipeline {
    agent any
    stages {
        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }
        stage('Run security tests') { 
            steps {
                bat 'npm audit'
            }
        }
        stage('Test') { 
            steps {
                bat 'npm test'
            }
        }
    }
}