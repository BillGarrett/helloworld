pipeline {
  agent any
  stages {
    stage('ls') {
      steps {
        sh '''whoami
pwd
ls -a
'''
        }
      }
    }
    stage('build') {
      agent {
        node {
          label 'make'
        }
        
      }
      steps {
        container('gcc') {
          sh '''which make
which gcc
echo okay
'''
        }
      }
    }
  }
}
