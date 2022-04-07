pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                npm install
            }
        }
        stage('Test') {
            steps {
                 jenkins/scripts/test
            }
        }
        stage('Deploy') {
            steps {
                 jenkins/scripts/deploy
            }
        }
    }
}
