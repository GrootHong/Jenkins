pipeline {
    agent any
environment { 
       username = 'Vito Hong'
    }
    stages {
        stage('Test') {
            steps {
                /* `make check` 在测试失败后返回非零的退出码；
                * 使用 `true` 允许流水线继续进行
                */
                sh 'make check || true' 
                echo "Hello Mr. ${username}"
            }
        }
stage('Example') {
            environment { 
                DEBUG_FLAGS = '-g'
            }
            steps {
                sh 'printenv'
            }
        }
    }
        
    
}