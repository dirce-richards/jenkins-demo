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
  
   stage('Development Tests') {
         when {
            beforeAgent true
            branch 'master'
         }
         steps {
            echo "Run the development tests!"
         }
      }
  }}
