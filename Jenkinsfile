pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        dir(path: 't5') {
          echo 'Print Message 1'
          sh 'npm init -f'
        }
      }
    }
  }
}
