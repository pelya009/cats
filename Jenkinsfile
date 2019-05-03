pipeline {
    agent { docker { image 'python:3.7.1' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'ls -la'
                sh 'python -m ./flask-app/app.py'
            }
        }
    }
}