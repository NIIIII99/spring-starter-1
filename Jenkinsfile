pipeline {
  agent {
    none
  }
  stages {
    stage('Test') {
      steps {
        mvnw.bat clean
      }
    }
    stage('Build') {
      steps {
        mvnw.bat package
      }
    }
  }
}
