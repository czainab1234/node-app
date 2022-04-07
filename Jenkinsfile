pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh './jenkins/scripts/test'
            }
        }
        stage('Deploy') {
            steps {
                sh './jenkins/scripts/deploy'
            }
        }
    }
}
