pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh 'mvnw clean check'
      }
    }
    stage('Build') {
      steps {
        echo 'build'
      }
    }
  }
}