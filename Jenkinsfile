pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'building'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
        stage('ExecuteSonarQubeReport') {
     nodejs(node: 'Nodejs7.8.0') {
        sh 'npm run sonar'
    }
      
        }
    }  
   }

