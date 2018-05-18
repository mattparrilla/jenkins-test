pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh '''new_version = $(git diff master:version.cmake version.cmake)
if [ -z "$new_version" ]
then
      return 1
else
      return 0
fi```
      }
    }
  }
}
