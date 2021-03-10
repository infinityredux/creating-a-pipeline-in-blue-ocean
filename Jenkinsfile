pipeline {
  agent any
  stages {
    stage('Preparation') {
      steps {
        sh 'npm install'
      }
    }

    stage('Tests') {
      when {
        branch 'master'
      }
      environment {
        CI = 'true'
      }
      steps {
        sh './jenkins/scripts/test.sh'
      }
    }

  }
}