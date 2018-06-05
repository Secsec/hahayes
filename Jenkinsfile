pipeline {
  agent any
  stages {
    stage('Initialize') {
      steps {
        git(url: 'https://github.com/Secsec/hahayes', branch: 'master')
        sh 'echo'
      }
    }
    stage('Checkout') {
      steps {
        sh 'echo'
      }
    }
    stage('Unit Tests') {
      steps {
        sh 'echo'
      }
    }
    stage('Build WAR') {
      steps {
        sh 'echo'
      }
    }
    stage('Build Image') {
      steps {
        sh 'echo'
      }
    }
    stage('Verify Image') {
      steps {
        sh 'echo'
      }
    }
    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            sh 'echo'
          }
        }
        stage('Deploy Load Injector') {
          steps {
            sh 'echo'
          }
        }
      }
    }
    stage('Load Test') {
      steps {
        sh 'echo'
      }
    }
  }
  environment {
    maven = ''
  }
}
