pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/ohk3726/trainer.git'
      }
    }

    stage('Build') {
      steps {
        tool 'gradle5'
      }
    }

    stage('Deploy') {
      steps {
        sh 'echo "Deploy Success"'
      }
    }

  }
}