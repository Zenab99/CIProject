pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage('Install dependencies') {
            steps {
                bat 'npm install'
            }
        }
        stage('Build ') {
            steps{
                bat 'npm run build'
            }
        }
        stage('Test') {
            steps {
                bat 'npm run test'
            }
        }
        stage('Deploy') {
            steps {
                bat 'npm run deploy'
            }
        }
    }
}