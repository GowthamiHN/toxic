pipeline {
    agent any

    stages {
        stage("default") {
            steps {
                sh 'sudo rm -rf /var/www/html/index.html'
            }
        }
        stage("custom page") {
            steps {
                sh 'sudo cp index.html /var/www/html/index.html'
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