pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('build') {
            steps {
            	sh 'pip3 install Django'
                sh 'python3 manage.py runserver'
            }
        }
    }
}
