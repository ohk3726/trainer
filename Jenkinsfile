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
        sh 'sudo Docker ps'
      }
    }

  }
}