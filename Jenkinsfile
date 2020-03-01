pipeline {
  agent any
  stages {
    stage('2nd') {
      parallel {
        stage('2nd') {
          steps {
            sh 'echo "Second Step"'
          }
        }

        stage('2.1') {
          steps {
            sh 'echo "Preparing Unit test environment"'
          }
        }

        stage('2.2') {
          steps {
            sh 'echo "Running Junit Testing......"'
          }
        }

      }
    }

    stage('Final Step') {
      steps {
        sh 'echo "Completed Pipeline"'
      }
    }

  }
}