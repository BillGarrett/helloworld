pipeline {
  agent any
  stages {
    stage('Hello') {
      parallel {
        stage('Hello') {
          steps {
            sh 'echo Hello, world!'
          }
        }
        stage('ls') {
          steps {
            sh '''whoami
pwd
ls -a
'''
          }
        }
      }
    }
  }
}