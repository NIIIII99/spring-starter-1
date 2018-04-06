pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh 'mvn -B -DskipTests clean package'
      }
    }
    stage('Build') {
      steps {
        echo 'build'
      }
    }
  }
}