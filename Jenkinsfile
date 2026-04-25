pipeline {
    agent any

    stages {
        stage("check ls") {
            steps {
                sh 'ls -a'
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