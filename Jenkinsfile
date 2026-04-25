pipeline {
    agent any

    stages {
        stage("check ls") {
            steps {
                sh 'ls -a'
            }
        }
        stage("check pwd") {
            steps {
                sh 'pwd'
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