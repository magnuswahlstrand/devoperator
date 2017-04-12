pipeline {
  agent any
  stages {
    stage('Build Flake') {
      steps {
        parallel(
          "Build Flake": {
            sh 'ls'
            
          },
          "Build Project CHEMU": {
            echo 'Hej :)'
            
          },
          "Build Project TRX-IF": {
            sleep 15
            
          }
        )
      }
    }
    stage('Test CHEMU') {
      steps {
        echo 'CHEMU'
      }
    }
    stage('') {
      steps {
        parallel(
          "": {
            mail(subject: 'Magnus', body: ':-D')
            
          },
          "Update part 1": {
            sleep 10
            
          }
        )
      }
    }
  }
}