pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        bat(script: 'mvnw.cmd clean', returnStatus: true, returnStdout: true)
      }
    }
    stage('Build') {
      steps {
        bat(script: 'mvnw.cmd install', returnStatus: true, returnStdout: true)
      }
    }
  }
}