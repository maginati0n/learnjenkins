pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                pip install -r requirements.txt
            }
        }
        stage("Test"){
            steps {
                echo "Test Stage" \
                python3 app.py
            }
        }
    }
}