pipeline {
    agent any
    parameters{
        string(name: 'appname', defaultValue: 'sanbox-hessian', descriptions: 'app name')
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
