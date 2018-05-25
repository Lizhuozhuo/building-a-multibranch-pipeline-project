pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        input(message: 'submit or cancel?', parameters: [choice(choices: ['master', 'release', 'dev'], description: '', name: 'branch'), text(defaultValue: '1', description: '', name: 'node num')])
        sh 'echo "Hello world!"'
        sh 'echo "test the patch"'
        sh 'echo "branch"'
        input 'test is pass or reject? (Click "Proceed" to continue)'
        sh 'echo "pass"'
      }
    }
  }
  parameters {
    string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
  }
}