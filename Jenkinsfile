pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building started..'
            }
        }
        stage('Test') {
            steps {
                sh 'netstat -nltup |grep 8080'
                echo 'Jenkins is Running!'
            }
        }
        stage('Deploy') {
            steps {
                sh 'cd /var/www/html-sample-app && sudo git pull'
            }
        }
    }
}

