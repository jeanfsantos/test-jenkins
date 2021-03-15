pipeline {
  agent any
  parameters {
    choice(
      name: 'Version',
      choices: ['patch', 'minor', 'major'],
      description: 'Escolha versão'
    )
    string(defaultValue: '', description: '', name: 'branch', trim: true)
  }
  stages {
    stage('Versão') {
      steps {
        echo "A versão é ${params.Version}"
      }
    }
  }
}