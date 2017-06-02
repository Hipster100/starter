pipeline {
  agent any

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
