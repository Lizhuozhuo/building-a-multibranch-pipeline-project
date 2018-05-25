pipeline {
    agent any
    stages {
        stage('Example') {
            input {
                message "Should we continue?"
                ok "Yes, we should."
                parameters {
                    string(name: 'PERSON', defaultValue: 'paas-sandbox-boss', description: '项目名')
                    string(name: 'env', defaultValue: 'master', description: '构建分支')
                    string(name: 'node num', defaultValue: '1', description: '部署节点数')
                }
            }
            steps {
                echo "Hello, ${PERSON}, nice to meet you."
            }
        }
    }
}
