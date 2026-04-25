pipeline {
    agent any

    stages {
        stage("check nginx") {
            steps {
                sh 'which nginx'
            }
        }
        stage("check list") {
            steps {
                sh 'ls'
            }
        }
    }
    post {
        success {
            echo "working"
        }
        failure {
            echo "failure"
        }
    }
}