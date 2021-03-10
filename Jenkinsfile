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
      steps {
        sh './jenkins/scripts/test.sh'
      }
    }

  }
}