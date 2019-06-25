pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage(' Installerar dependencies') {
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
                bat 'npm run Testing..'
            }
        }
        stage('Deploy') {
            steps {
                bat 'npm run Deploying'
            }
        }
    }
}