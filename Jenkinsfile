pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'I want to build'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'I want to Test'
          }
        }

        stage('Deploy') {
          steps {
            echo 'Deployed'
          }
        }

      }
    }

  }
}