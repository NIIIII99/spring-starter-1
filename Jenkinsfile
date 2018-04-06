pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh 'mvnw -B -DskipTests clean package'
      }
    }
    stage('Build') {
      steps {
        echo 'build'
      }
    }
  }
}