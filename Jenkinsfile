pipeline {
    agent { docker { image 'python:3.7.1' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'ls -la'
                sh 'python -m ensurepip'
                sh 'pip install -r flask-app/requirements.txt'
                sh 'python flask-app/app.py'
            }
        }
    }
}