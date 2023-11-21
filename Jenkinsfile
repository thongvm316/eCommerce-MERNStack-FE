pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        script {
          git 'https://github.com/your/repo.git'
        }
      }
    }

    stage('Build') {
      steps {
        script {
          nodejs('nodejs') {
            sh 'npm install'
            sh 'npm run build'
          }
        }
      }
    }

    stage('Test') {
      steps {
        script {
          nodejs('nodejs') {
            sh 'npm test'
          }
        }
      }
    }

    stage('Deploy') {
      steps {
        // Add deployment steps here
      }
    }
  }
}
