pipeline {
  agent any

  tools {
        nodejs 'Default'
    }

  environment {
    CI = 'true'
  }

  stages {

    stage('Install') {
      steps {
        sh 'npm install'
      }
    }

    stage('Test') {
      steps {
        sh 'npm run test -- --coverage'
      }
    }
  }
}
