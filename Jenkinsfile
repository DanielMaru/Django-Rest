pipeline {
    agent {
        docker {
            image 'python:3-alpine' 
            args '-p 3000:3000' 
        }
    }
    environment {
        CI = 'true' 
    }
    stages {
        stage('Build') { 
            steps {
                sh 'pip' 
            }
        }
        stage('Test') { 
            steps {
                sh 'chmod +x ./jenkins/scripts/test.sh'
                sh './jenkins/scripts/test.sh' 
            }
        }
    }
}
