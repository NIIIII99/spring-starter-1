pipeline {
  agent {
    none
  }
  stages {
    stage('Test') {
      steps {
        mvnw.cmd clean
      }
    }
    stage('Build') {
      steps {
        mvnw.cmd package
      }
    }
  }
}
