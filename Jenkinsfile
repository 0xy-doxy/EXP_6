pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        echo 'Cloning repository...'
        checkout scm
      }
    }

    stage('Build') {
      steps {
        echo 'Building project...'
        sh 'ls -l'
      }
    }

    stage('Test') {
      steps {
        echo 'Running validation...'
        sh 'echo "No tests yet"'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying web app...'
        sh 'echo "Files deployed successfully"'
      }
    }
  }

  post {
    success {
      echo '✅ Pipeline completed successfully!'
    }
    failure {
      echo '❌ Pipeline failed!'
    }
  }
}
