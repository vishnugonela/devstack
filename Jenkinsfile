pipeline {
  agent any
  stages {
    stage('1st') {
      steps {
        sh 'echo "Hello World"'
        sleep 2
      }
    }
    stage('2nd') {
      steps {
        sh 'echo "Second Step"'
      }
    }
    stage('Final') {
      steps {
        sh 'echo "DONE"'
      }
    }
  }
}