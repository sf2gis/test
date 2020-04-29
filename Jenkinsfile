pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo "build"'
      }
    }

    stage('test') {
      environment {
        CI = 'true'
      }
      steps {
        sh '''pwd
./test.sh'''
      }
    }

  }
}