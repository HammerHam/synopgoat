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
          sh './mvn org.sonarsource.scanner.maven:sonar-maven-plugin:3.9.1.2184:sonar'
            }
          }
       }
    }
}


