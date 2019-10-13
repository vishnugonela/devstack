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
    stage('Third') {
      steps {
        sh '''echo "Docker step"
yum install docker -y '''
      }
    }
    stage('Final Step') {
      steps {
        sh 'echo "Completed Pipeline"'
      }
    }
  }
}