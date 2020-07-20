pipeline {
    agent {
        label 'docker'
    }
    stages {
        stage('Zero') {
            steps {
                echo 'Stage 0'
            }
        }
        parallel {
            stage('Unit Tests') {
                steps {
                    echo 'Unit tests...'
                }
            }
            stage('Integration tests') {
                steps {
                    echo 'Integration tests...'
                }
            }
        }

    }
}