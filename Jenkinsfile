pipeline {
    agent any
    if (XD_Env_BUS_Update_Start == 'true') {
    println "XD_Env_BUS_Update_Start - 更新"
    build job: 'XD_Env_BUS_Update_Start', parameters: [string(name: 'Env', value: BD_Env), string(name: 'BD_Dir', value: BD_Dir)]
    } else {
    println "XD_Env_BUS_Update_Start - 不更新"
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello world!"'
            }
        }
    }
}
