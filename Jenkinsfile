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
        sh 'cd /root'
        dir(path: './t6') {
          echo 'Print Message 1'
          echo pwd()
          sh 'npm init -f'
          input 'Finished using the web site? (Click "Proceed" to continue)'
        }

        sh 'TTT="${PWD}"'
        sh 'echo "${TTT}"'
        pwd(tmp: true)
        writeFile(file: 'ttt.txt', text: 'happy')
        pwd()
        writeFile(file: 'ttt2.txt', text: 'happy2')
        echo pwd()
        echo pwd(tmp: true)
      }
    }
  }
}
