pipeline {
  agent none
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
        sh 'mvn clean install'
      }
    }

    stage('Test') {
      steps {
        echo 'Testing..'
        sh 'mvn test'
      }
    }

    stage('Package') {
      steps {
        echo 'Packaging'
        sh 'mvn package'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deloying...'
      }
    }

  }
}