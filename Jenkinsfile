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
        sh 'mkdir -p /root/t6'
        dir(path: '/root/t6') {
          echo 'Print Message 1'
          sh 'npm init -f'
          input 'Finished using the web site? (Click "Proceed" to continue)'
        }
      }
    }
  }
}
