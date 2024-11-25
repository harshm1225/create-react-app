pipeline {
  agent any

  tools {nodejs "node"}

  stages {
    stage('Install Dependencies') {
      steps {
        sh 'npm info'
        sh 'npm install'
      }
    }
    stage('Build') {
      steps {
        sh 'npm run build'
      }
    }
    stage('Test') {
      steps {
        sh 'npm test'
      }
    }
  }
}