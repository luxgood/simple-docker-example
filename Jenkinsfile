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

        stage('Integration tests') {
            steps {
                echo 'Testing...'
            }
        }

        stage('Kill grid') {
            steps {
                sh 'docker-compose down'
            }
        }
    }
}