pipeline {
    agent {
        label 'docker'
    }
    stages {
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