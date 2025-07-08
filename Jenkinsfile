
pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo 'Building...'
                sh 'mvn clean package'
            }
        }
        stage ('test') {
            steps {
                echo 'Testing...'
            }
        }
        stage ('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'mvn deploy'
            }
        }
        stage ('Cleanup') {
            steps {
                echo 'Cleaning up...'
                sh 'mvn clean'
            }
        }
    }
}
