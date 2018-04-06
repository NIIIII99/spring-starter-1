pipeline {
  agent {
    docker {
      image 'maven:3-alpine' 
      args '-v /root/.m2:/root/.m2' 
    }
  }
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
