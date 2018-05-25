pipeline {
    agent any
    parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
    }
    stages {
        stage('Build') {
            steps {
                input id: '1', message: 'submit or cancel?', ok: 'submit', parameters: [choice(choices: ['master', 'release', 'dev'], description: '', name: 'branch'), text(defaultValue: '1', description: '', name: 'node num')], submitter: 'admin', submitterParameter: 'branch'
                sh 'echo "Hello world!"'
                sh 'echo "test the patch"'
                sh 'echo "branch"'
                input message: 'test is pass or reject? (Click "Proceed" to continue)'
                sh 'echo "pass"'
            }
        }
    }
}
