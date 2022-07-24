pipeline {
    agent any
    stages {
        stage('githup') {
            environment {
                SERVICE_CREDS = credentials('git')
            }
            steps {
                sh 'echo "Service user is $SERVICE_CREDS_USR"'
             

            }
        }
        stage('docker hup') {
            environment {
                SSH_CREDS = credentials('doc')
            }
            steps {
             
                sh 'echo "SSH user is $SSH_CREDS_USR"'
              
            }
        }
    }
}
