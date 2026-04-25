pipeline {
    agent any

    stages {
        stage("install nginx") {
            steps {
                sh 'apt install nginx -y'
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