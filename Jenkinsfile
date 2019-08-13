pipeline {
    agent  any
    tools {nodejs "node"}
       
    stages {
        stage('install dependencies') { 
            steps {
                bat 'npm install' 
            }
        }
        
        stage('Build production files') { 
            steps {
                bat 'npm run build'  
            }
        }
        stage('Test'){
            steps {
                bat 'npm run test'
            }
        }
        stage('Deploy'){
            steps {
                bat 'npm run deploy'
        }
    }
}
}