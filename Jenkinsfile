pipeline {
    agent any

    stages {
        stage("check nginx") {
            steps {
                sh 'sudo which nginx'
            }
            post {
                success {
                    echo "working check nginx"
                }
                failure {
                    echo "failure check nginx"
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