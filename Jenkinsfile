pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh './gradlew build'
      }
    }

    stage('docker stop') {
      steps {
        sh 'docker stop trainer'
      }
    }

    stage('docker rm') {
      steps {
        sh 'docker rm trainer'
      }
    }

    stage('docker build') {
      steps {
        sh 'docker build -t trainer .'
      }
    }

    stage('docker run') {
      steps {
        sh 'docker run -d -p 9000:8081 --name trainer trainer'
      }
    }

  }
}