@Library('jenkins-shared-library') _

pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        buildNodeApp()
      }
    }

    stage('Deploy') {
      steps {
        deployToBeanstalk('DevopsFrontendTest', 'Devopsfrontendtest-env', '1.0.0')
      }
    }
  }
}
