pipeline {
  agent any
  stages {
    stage('Version') {
      steps {
        sh '''new_version = $(git diff origin/master:version.cmake version.cmake)
if [ -z "$new_version" ]
then
      return 1
else
      return 0
fi'''
      }
    }
  }
}