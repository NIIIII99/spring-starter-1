pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        bat(script: 'mvnw.cmd clean', returnStatus: true, returnStdout: true)
      }
    }
    stage('Package') {
      steps {
        bat(script: 'mvnw.cmd package', returnStatus: true, returnStdout: true)
      }
    }
    stage('Deploy Dev Sevice') {
      steps {
        bat 'service spring-starter stop'
        bat 'java -jar spring-starter-0.0.1-SNAPSHOT.jar'
      }
    }
  }
}