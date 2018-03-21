pipeline {
  agent any
  stages {
    stage('Install') {
      steps {
        sh 'npm i -g yarn'
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