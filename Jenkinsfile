pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/czainab1234/node-app.git'
      }
    }
     
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
  }
}
