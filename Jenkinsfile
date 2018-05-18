pipeline {
  agent any
  stages {
    stage('Version') {
      steps {
        sh '''if [ -z "$(git diff origin/master:version.cmake version.cmake)" ]
then
      return 1
else
      return 0
fi'''
      }
    }
  }
}