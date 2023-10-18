pipeline {
  agent any
  stages {
    stage('SCM CheckOut') {
      steps {
        git(url: 'https://github.com/HaithamKhalifa/demo1.git', branch: 'master')
      }
    }
   stage('Bulid Image') {
      steps {
        sh 'podman build -t .'
      }
  }
}
}