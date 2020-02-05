pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'build getting executed'
          }
        }

        stage('parallel_pipeline') {
          steps {
            echo 'parallel code written'
          }
        }

        stage('parallel_pipeline2') {
          steps {
            echo 'parallel pipeline2 created'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy the code on testing server'
      }
    }

  }
}