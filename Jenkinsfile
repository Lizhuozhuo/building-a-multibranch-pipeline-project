pipeline {
    agent any
    stages {
        input id: '1', message: 'runner?', ok: 'submit', 
        parameters: [string(defaultValue: 'boss', description: '应用名', name: 'appname', trim: false), run(description: '测试结果', filter: 'COMPLETED', name: 'test_result', projectName: 'master'), choice(choices: ['master', 'release', 'dev', 'release_1'], description: '', name: 'branch'), text(defaultValue: '1', description: '', name: '节点数')], submitter: 'admin'
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
