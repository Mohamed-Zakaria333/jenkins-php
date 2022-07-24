pipeline {
    agent any

    stages {
        stage('Build') {
            steps{
                 withCredentials([usernamePassword(credentialsId: 'git', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {
                 sh 'echo $PASSWORD'
                 echo USERNAME
                 echo "username is $USERNAME"
                 }
                echo 'Building.. zakaria from git hup'
            }
        }
        stage('Test') {
            steps {
                 withCredentials([usernamePassword(credentialsId: 'git', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {
                 sh 'echo $PASSWORD'
                 echo USERNAME
                 echo "username is $USERNAME"
                 }
                 echo'Testing.. zakaria from git hup'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying.... zakaria from git hup'
            }
        }
    }
}
