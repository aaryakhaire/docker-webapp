pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                bat 'docker build -t aarya-webapp .'
            }
        }

        stage('Run Container') {
            steps {
                bat 'docker run -d -p 8081:80 aarya-webapp'
            }
        }
    }
}
