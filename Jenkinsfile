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
        
       stage('SonarQube analysis') {
//    def scannerHome = tool 'SonarScanner 4.7.0';
        steps{
        withSonarQubeEnv('sonarqube-7.9.6') { 
        // If you have configured more than one global server connection, you can specify its name
//      sh "${scannerHome}/bin/sonar-scanner"
        sh "mvn sonar:sonar"
    }
        }
        } 
            
    }
}
