pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Checkout...'
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'mvn clean install' // Run Maven build commands
            }
        }
        
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'mvn test' // Run Maven test commands
            }
        }
        
        stage('Package') {
            steps {
                echo 'Packaging'
                sh 'mvn package' // Run Maven package commands
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deloying...'
            }
        }
    }
}