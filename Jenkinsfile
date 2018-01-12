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
    stage('Write') {
      steps {
        timestamps() {
          writeFile(file: 'Test', text: 'WriteFile')
        }
        
      }
    }
    stage('CheckWrite') {
      steps {
        fileExists 'Writefile2'
      }
    }
  }
}