pipeline {
    agent any
        stages{
            stage('One'){
                steps{
                    echo 'Hello there in step One of Stage One'
                }
            }
            stage('Two'){
                steps{
                    docker{
                        docker container ls -a
                    }
                }
            }
            stage('With docker'){
                agent{
                    docker
                }
                steps{
                    echo "Hello"
                    docker docker-compose up
                }
            }
        }



}