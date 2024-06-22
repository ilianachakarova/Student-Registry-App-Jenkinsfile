pipeline{
    agent any
    stages{
        stage("Check version"){
            steps{
                bat 'npm install'
            }
        }
        stage("NPM Audit"){
            steps{
                bat 'npm audit'
            }
        }
        stage("Run tests"){
            steps{
                bat 'npm test'
            }
        }
        stage("Deploy"){
            steps{
                bat 'docker build -t chakarova94/studentsapp .'
            }
        }
    }
}