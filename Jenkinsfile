pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello build'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Hello Test'
          }
        }

        stage('Deploy') {
          steps {
            echo 'Hello Deploy'
          }
        }

      }
    }

  }
}
