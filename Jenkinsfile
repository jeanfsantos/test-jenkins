pipeline {
  agent any
  stages {
    stage('Params') {
      steps {
        echo 'A versão é ${params.Version}'
        echo 'A branch é ${params.Branch}'
      }
    }
    stage('checkout') {
        steps {
            git branch: params.Branch,
            credentialsId: '96c4ca8d-d1d1-465e-9642-7468e056c50e',
            url: 'https://github.com/jeanfsantos/test-jenkins.git'
        }
    }
  }
}