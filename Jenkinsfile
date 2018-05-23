pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/Secsec/hahayes', branch: 'master')
        sh 'mvn package'
        stash 'yes-0.0.1-SNAPSHOT.jar'
      }
    }
    stage('Build Image') {
      steps {
        unstash 'yes-0.0.1-SNAPSHOT.jar'
        sh 'oc start-build yes --from-file=target/yes-0.0.1-SNAPSHOT.jar --follow'
      }
    }
  }
  tools {
    maven 'maven.3.5.3'
  }
  environment {
    maven = ''
  }
}