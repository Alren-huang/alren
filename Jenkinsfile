pipeline {
  agent any
  stages {
    stage('aaa') {
      steps {
        sh 'echo "aa"'
        input(message: 'fafafa', id: 'aa', submitter: 'afa', submitterParameter: 'aaa', ok: 'a')
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
            
          },
          "": {
            sh 'echo ""'
            echo 'aaaa'
            readFile '/'
            
          }
        )
      }
    }
  }
}