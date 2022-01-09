pipeline {
    agent any
	
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
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
   	stage('Scan') {
	    steps {
                withSonarQubeEnv(installationName: 'sq1') { 
          #!/bin/bash mvn clean sonar:sonar
            }
          }
       }
    }
}


