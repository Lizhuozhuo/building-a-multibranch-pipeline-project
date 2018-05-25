pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello world!"'
                input message: 'Finished using the web site? (Click "Proceed" to continue)'
                sh 'echo "reject"'
            }
        }
    }
}
