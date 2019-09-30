pipeline {
  agent any
  stages {
    stage('test1') {
      environment {
        test = 'test'
      }
      parallel {
        stage('test1') {
          steps {
            echo 'test er'
          }
        }
        stage('') {
          steps {
            sleep 1
          }
        }
        stage('') {
          steps {
            sh 'ls -aih'
          }
        }
      }
    }
    stage('') {
      steps {
        sh 'ls'
      }
    }
    stage('test') {
      steps {
        sh 'echo \'hello world!\''
      }
    }
  }
}