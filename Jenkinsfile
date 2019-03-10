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
        dir(path: 'tttt') {
          echo 'Print Message 1'
          pwd(tmp: false)
          sh 'npm init -f'
        }
      }
    }
  }
}
