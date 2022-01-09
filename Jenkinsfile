pipeline {
    agent { docker { image 'node:16.13.1-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'node --version'
            }
        }
    }
}

pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'set'
            }
        }
    }
}
