pipeline {
    agent any

    stages {
        stage("install nginx") {
            steps {
                sh 'sudo apt install nginx -y'
            }
            post {
                success {
                    echo "working install nginx"
                }
                failure {
                    echo "failure install nginx"
                }
            }
        }
        stage("check nginx") {
            steps {
                sh 'sudo systemctl status nginx'
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