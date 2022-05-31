pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'pwd'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'for test'
          }
        }

        stage('preprod') {
          steps {
            sh 'ls'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'finally done'
      }
    }

  }
}