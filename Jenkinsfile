pipeline{
    agent any
    stages{
        stage("CodeScan"){
            steps{
                sh 'trivy --version'
                sh 'trivy fs . -o result.html'
                sh 'cat result.html'
            }
        }
        stage("dockerImageBuild"){
            steps{
               sh 'docker -v' 
            }
        }
        stage("pushImage"){
            steps{
                sh 'docker ps'
            }
        }

    }
}