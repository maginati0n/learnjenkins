pipeline {
    agent { docker { image 'python:3.10.7-alpine' } }
    stages {
        stage("Build") {
            steps {
               sh pip install -r requirements.txt
            }
        }
        stage("Test"){
            steps {
                echo "Test Stage" \
                sh python3 app.py
            }
        }
    }
}