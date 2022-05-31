pipeline {
  agent any
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh '''pwd
date'''
          }
        }

        stage('prod') {
          steps {
            sh '''ls
u
whoami'''
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'it is deploy'
      }
    }

  }
}