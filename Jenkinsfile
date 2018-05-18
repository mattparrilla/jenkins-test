pipeline {
  agent any
  stages {
    stage('Version') {
      steps {
        sh '''git branch -r
new_version = $(git diff master:version.cmake version.cmake)
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