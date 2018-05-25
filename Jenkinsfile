pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello world!"'
                input message: 'test is pass or reject? (Click "Proceed" to continue)'
                sh 'echo "pass"'
            }
        }
    }
}
