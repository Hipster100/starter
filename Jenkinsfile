pipeline {
  agent any

  tools {
        nodejs 'Node 6.x'
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
