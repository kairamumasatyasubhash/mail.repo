
pipeline {
    agent slave {
        label 'java-slave'
    }
    stages {
        stage ('Build') {
            steps {
                echo 'Building...'
                sh 'mvn clean package'
            }
        }
        satge ('test') {
            steps {
                script {
                echo 'Testing...'
                  }
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
