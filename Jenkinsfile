pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        bat 'mvnw.cmd clean'
      }
    }
    stage('Build') {
      steps {
        bat 'mvnw.cmd package'
      }
    }
  }
}