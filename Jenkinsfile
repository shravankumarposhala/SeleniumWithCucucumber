pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        cucumber '*'
      }
    }
    stage('QA') {
      steps {
        sleep(time: 10, unit: 'SECONDS')
      }
    }
    stage('Pre-Prod') {
      steps {
        echo 'completed'
      }
    }
    stage('Prod') {
      steps {
        echo 'deployed'
      }
    }
  }
  environment {
    PreProd = '10'
  }
}
