pipeline{
     agent {
                docker {
                    image 'node:current-alpine3.19'
                    reuseNode true
                }
            }
    stages{
        stage("Check version"){
            steps{
                sh 'node --version'
            }
        }
    }
}