pipeline {
    agent any
    
    stages {
        stage('Build') { 
            steps {
                sh 'sudo apt-get install npm -y'
                git 'https://github.com/abhikedia/react-unit-test-practice.git'
                sh 'npm install' 
            }
        }
        
        stage('Test') {
            steps {
                sh 'npm run test'
            }
        }
    }
}
