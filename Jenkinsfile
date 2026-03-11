pipeline {
    agent any

    stages {

        stage('Secret Scan') {
            steps {
                sh 'trufflehog git .'
            }
        }

        stage('Static Code Scan') {
            steps {
                sh 'sonar-scanner'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t secure-app .'
            }
        }

        stage('DAST Scan') {
            steps {
                sh 'zap-baseline.py -t http://localhost:5000'
            }
        }

    }
}
