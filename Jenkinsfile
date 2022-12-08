pipeline {
  agent {
    node {
      label 'built-in'
    }

  }
  stages {
    stage('Source') {
      steps {
        git(url: 'https://github.com/ohk3726/trainer.git', branch: '*/marster')
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