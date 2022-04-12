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
             nodejs(nodeJSInstallationName: 'nodejs16.14.2') {
             sh 'npm run sonar'
    }
          }
      }
          
      
            
    }
}
