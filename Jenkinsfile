pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                sh 'ssh 172.31.42.50 "rm palette-generator && mkdir palette-generator"'
                sh 'scp -r . 172.31.42.50:/home/jenkins/palette-generator'
                sh 'ssh 172.31.42.50 < scripts/ssh-connect.sh'
            }
        }
    }
}