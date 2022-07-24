pipeline {
    agent any

    stages {
        stage('Build') {
            environment{
                cre=credentials('git')
            }
            steps {
                echo 'Building.. zakaria from git hup'
                echo "${cre.Username}"
      
            }
        }
        stage('Test') {
             environment{
                cre=credentials('doc')
            }
            steps {
                echo 'Testing.. zakaria from git hup'
                echo "${cre.Username}"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying.... zakaria from git hup'
            }
        }
    }
}
