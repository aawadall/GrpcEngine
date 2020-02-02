pipeline {
    agent any
    stages {
        stage('Predeploy') {
            steps {
                sh 'apt-get update'
                sh 'apt-get install install apt-transport-https'
                sh 'apt-get update'
                sh 'apt-get install dotnet-sdk-3.1'
            }
        }
        stage('Build') {
            steps {
                sh 'dotnet build'
            }
        }
    }
}