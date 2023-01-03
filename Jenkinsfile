pipeline {
    agent { docker { image 'python:3.10' } }
    stages {
        stage('test') {
            steps {
                sh 'python --version'
                sh 'pip --version'
            }
        }
        stage('build'){
            steps {
                sh 'pip install -r requirements.txt'
            }
        }
        stage('run'){
            steps{
                sh 'python app.py'
            }
        }
    }
}