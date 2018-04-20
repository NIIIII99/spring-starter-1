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
        bat(script: 'mvnw.cmd package', returnStatus: true, returnStdout: true)
        bat(script: 'mvnw.cmd build', returnStatus: true, returnStdout: true)
      }
    }
  }
}