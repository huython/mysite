pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('build') {
            steps {
            	sh 'virtualenv env -p python3.5'
            	sh '. env/bin/activate'
            	sh 'env/bin/pip install -r requirements.txt'
                sh 'env/bin/python3.5 manage.py runserver'
            }
        }
    }
}
