pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                sh 'ssh 172.31.42.50 < scripts/ssh-connect.sh'
            }
        }
    }
}