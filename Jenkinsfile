pipeline {
  agent any
  stages {
    stage('Version') {
      steps {
        sh '''if [ -z "$(git diff origin/master:version.cmake version.cmake)" ]
then
  echo "Your version.cmake is the same as master"
  echo "You need a new version in order to merge"
  return 1
fi'''
      }
    }
  }
}