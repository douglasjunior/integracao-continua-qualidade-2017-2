pipeline {
  agent any
  stages {
    stage('Install') {
      steps {
        sh '''export PATH=/var/jenkins_home/tools/jenkins.plugins.nodejs.tools.NodeJSInstallation/Node8/bin:$PATH
yarn install'''
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