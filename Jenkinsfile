pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    } 
    stages {

        stage('Deliver') {
            steps {
               
                sh "flask --version"
                sh "gunicorn --bind 0.0.0.0:8000 sources/server:app"

            }

        }


    }
}

