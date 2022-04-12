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
          steps{
             nodejs(nodeJSInstallationName: 'nodejs17.8.0') {
             sh 'npm run sonar'
    }
          }
      }
          
      
            
    }
}
