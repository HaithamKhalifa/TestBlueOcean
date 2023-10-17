pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'this is a test Build Step'
      }
    }

    stage('Test Stages') {
      parallel {
        stage('test1') {
          steps {
            echo 'test1 success'
          }
        }

        stage('test2') {
          steps {
            echo 'test2 success'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy success'
      }
    }

  }
}