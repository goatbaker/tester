pipeline {
  agent any
  stages {
    stage('Print') {
      parallel {
        stage('Print') {
          steps {
            echo 'This is sweet'
          }
        }
        stage('Print2') {
          steps {
            echo 'I feel alive'
          }
        }
      }
    }
  }
}