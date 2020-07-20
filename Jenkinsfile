pipeline {
    agent {
        label 'docker'
    }
    stages {
        stage('Build grid') {
            steps {
                sh 'docker-compose up'
            }
        }
    }
}