pipeline {
    agent any

    stages {
        stage("check jenkins") {
            steps {
                sh 'systemctl status jenkins'
            }
            post {
                success {
                    echo "working check jenkins"
                }
                failure {
                    echo "failure check jenkins"
                }
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