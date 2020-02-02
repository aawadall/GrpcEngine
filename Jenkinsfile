pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git credentialsId: 'aawadall', url: 'https://github.com/aawadall/GrpcEngine.git', branch: 'master'
            }
        }
        
        stage('Restore Packages') {
            steps {
                bat "dotnet restore"
            }
        }
        stage('Build') {
            steps {
                sh 'dotnet build'
            }
        }
    }
}