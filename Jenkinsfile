pipeline {
  agent any
  parameters {
    choice(
      name: 'Version',
      choices: ['patch', 'minor', 'major'],
      description: 'Escolha versão'
    )
  }
  stages {
    stage('Versão') {
      steps {
        echo "A versão é ${params.Version}"
      }
    }
  }
}