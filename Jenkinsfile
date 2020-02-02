pipeline {
    agent any
    stages {
        stage('Predeploy') {
            steps {
                sh 'echo "Test"'
            }
        }
        stage('Build') {
            steps {
                sh 'dotnet build'
            }
        }
    }
}