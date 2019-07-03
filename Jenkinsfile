pipeline {
  agent any
  stages {
    stage('first') {
      steps {
        sh 'ls'
      }
    }
    stage('second') {
      parallel {
        stage('second') {
          steps {
            echo 'second'
          }
        }
        stage('third') {
          steps {
            echo 'third'
          }
        }
      }
    }
  }
}