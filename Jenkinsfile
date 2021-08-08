pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                /* `make check` 在测试失败后返回非零的退出码；
                * 使用 `true` 允许流水线继续进行
                */
                sh 'make check || true' 
	def username = 'Vito Hong'
                echo "Hello Mr. ${username}"
            }
        }
stage('Example') {
            steps {
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            }
        }
    }
        
    
}