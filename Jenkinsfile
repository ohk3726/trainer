pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'ls -al'
      }
    }

    stage('Pre Docker Delete') {
      steps {
        sh '''pwd

docker ps'''
      }
    }

  }
}