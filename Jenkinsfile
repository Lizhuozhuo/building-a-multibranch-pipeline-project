pipeline {
    agent any
    parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello world!"'
                sh 'echo "test the patch"'
                sh 'echo "branch"'
                input message: 'test is pass or reject? (Click "Proceed" to continue)'
                sh 'echo "pass"'
            }
        }
    }
}
