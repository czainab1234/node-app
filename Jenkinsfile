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
             nodejs(nodeJSInstallationName: 'nodejs15.2.01') {
             sh 'npm run sonar'
    }
          }
      }
          
      
            
    }
}
