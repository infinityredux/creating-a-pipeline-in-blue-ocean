pipeline {
  agent any
  stages {
    stage('Preparation') {
      steps {
        sh 'npm install'
      }
    }

    stage('Tests') {
      steps {
        sh './jenkins/scripts/test.sh'
      }
    }

  }
}