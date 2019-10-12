pipeline {
  agent any
  stages {
    stage('Check Out SVN') {
      steps {
        echo 'Checking Out SVN'
      }
    }
    stage('Build') {
      steps {
        echo 'Building'
      }
    }
    stage('Test') {
      steps {
        echo 'Testing'
      }
    }
    stage('Email') {
      steps {
        emailext(subject: 'Jenkins', body: 'Hey This is Jenkins!!', to: 'david.tran@wdc.com')
      }
    }
    stage('Release') {
      steps {
        echo 'releasing!!!'
      }
    }
  }
}