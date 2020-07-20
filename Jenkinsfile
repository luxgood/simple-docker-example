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
                    input('Do you want to prroceed?')
                }
            }
            stage('Three'){
                when{
                    not{
                        branch "master"
                    }
                    steps{
                        echo "Hello"
                    }
                }
            }
        }



}