#!/usr/bin/env groovy
pipeline{
    agent {
        docker {
            image 'python:3-alpine' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'pip' 
            }
        }
    }
}