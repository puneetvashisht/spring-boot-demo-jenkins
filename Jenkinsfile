pipeline {
    agent any
    
    stages {
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
                // Add your deployment steps here
            }
        }
    }
}