pipeline{
    agent any
    stages{
        stage("stage1"){
            steps{
                sh "pwd"
                sh 'echo "stage1-clone" '
            }
        }
        stage("test-stage"){
            steps{
               sh 'echo "test-stage" ' 
            }
        }
        stage("create-file"){
            steps{
                sh 'touch test-${BUILD_ID}'
            }
        }

    }
}