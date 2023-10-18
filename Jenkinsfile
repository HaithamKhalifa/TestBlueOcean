pipeline {
  agent any
  stages {
    stage('SCM CheckOut') {
      steps {
        git(url: 'https://github.com/HaithamKhalifa/hapi-fhir-jpaserver-starter.git', branch: 'master')
      }
    }

    stage('Bulid Image') {
      steps {
        sh 'podman build -t .'
      }
    }

  }
}