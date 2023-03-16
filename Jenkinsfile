@Library('jenkins-shared-library') _

pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        nodejsBuild()
      }
    }

    stage('Deploy') {
      steps {
        deployToBeanstalk('my-app', 'my-env', '1.0.0')
      }
    }
  }
}
