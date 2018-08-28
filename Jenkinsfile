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
        git(url: 'https:/github.com/shravankumarposhala/SeleniumWithCucucumber.git, branch: 'mvn')
      }
    }
  }
  environment {
    PreProd = '10'
  }
}
