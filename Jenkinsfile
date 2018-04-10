pipeline {
  agent {
    docker {
      image 'maven:alpine'
    }
    
  }
  stages {
    stage('stage0') {
      steps {
        sh 'mvn -v'
      }
    }
  }
}