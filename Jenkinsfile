pipeline {
  agent any
  stages {
    stage('aaa') {
      steps {
        sh 'echo "aa"'
      }
    }
    stage('aa') {
      steps {
        parallel(
          "aa": {
            sh 'ls'
            
          },
          "vv": {
            sh 'ls'
            
          }
        )
      }
    }
  }
}