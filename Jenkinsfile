pipeline {
    agent {
        label 'docker'
    }
    stages {
        stage('ParallelStage'){
            parallel {
                stage('Unit Tests stage') {
                    steps {
                        echo 'Unit tests...'
                    }
                }
                stage('Integration tests stage') {
                    steps {
                        echo 'Integration tests...'
                    }
                }
            }
        }

    }
}