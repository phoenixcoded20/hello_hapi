#!/usr/bin/env groovy

pipeline {
     
    agent {
        docker {
            image 'node'
            args '-u root'
        }
    }
    
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'npm install'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'cd /var/www/html/'
                sh 'ls'
            }
        }
        
    }
}
