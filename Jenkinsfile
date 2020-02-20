pipeline {
  agent none
  stages {
    stage('1st') {
      parallel {
        stage('1st') {
          steps {
            sh 'echo "Hello World"'
            sleep 2
          }
        }

        stage('1.1') {
          steps {
            sh 'echo "Parallel Process Step"'
          }
        }

      }
    }

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

    stage('Third') {
      steps {
        sh '''echo "Docker step"
yum install docker -y || echo "Not able install docker"'''
      }
    }

    stage('Final Step') {
      steps {
        sh 'echo "Completed Pipeline"'
      }
    }

  }
}