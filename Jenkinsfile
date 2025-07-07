pipeline {
    agent any
    stages {
        stage('sucess the code') {
            steps {
                echo "This is a successful pipeline execution"
            }
        }
        stage ('bulding the applicsatiom') {
            steps {
                echo "Building the application"
            }
        }
        post {
            sucess {
                mail bcc: '',body: 'The build was successful!', 
                     cc: '', from: '', replyTo: '', subject: 'Build Success Notification', 
                     to: 'classdevops378@gmail.com'
            }
            failure {
                mail bcc: '', body: 'The build failed. Please check the logs.', 
                     cc: '', from: '', replyTo: '', subject: 'Build Failure Notification', 
                     to: 'classdevops378@gmail.com'
        }
    }
}
