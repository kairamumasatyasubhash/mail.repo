pipeline {
    agent any 
    stages {
        stage ('Build') {
            steps {
                Retry(1) {
                    echo "Welcome to jenkins Pipelines"
                    error "This is like a Failure"
                }
                    echo "*** I Retryed for 4 times ***"
            }
        }

        }
    }
