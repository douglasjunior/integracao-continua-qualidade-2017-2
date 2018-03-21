pipeline {
  agent any
  stages {
    stage('Install') {
      steps {
        sh 'yarn install'
      }
    }
    stage('Lint') {
      steps {
        sh 'yarn lint'
      }
    }
    stage('Test') {
      steps {
        sh 'yarn test'
      }
    }
  }
}