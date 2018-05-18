pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh 'git branch'
        sh 'echo $currentBuild.description'
      }
    }
  }
}