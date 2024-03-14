pipeline {
    agent {
        docker {
            image 'maven:3.8.4' // Specify the Maven Docker image version
            args '-v $HOME/.m2:/root/.m2' // Mount the local Maven repository to the Docker container
        }
    }
    
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install' // Run Maven build commands
            }
        }
        
        stage('Test') {
            steps {
                sh 'mvn test' // Run Maven test commands
            }
        }
        
        stage('Package') {
            steps {
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