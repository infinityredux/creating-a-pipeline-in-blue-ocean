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
        branch 'feature/does-not-exist'
      }
      steps {
        sh './jenkins/scripts/test.sh'
      }
    }

  }
}
