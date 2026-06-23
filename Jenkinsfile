pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'docker build -t jenkins-demo .'
            }
        }

        stage('Test') {
            steps {
                bat 'docker run --rm jenkins-demo'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Application Deployed Successfully'
            }
        }
    }
}