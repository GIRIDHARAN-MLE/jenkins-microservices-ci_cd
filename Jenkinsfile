pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Build"
            }
        }
        stage('TEST') {
            steps {
                echo "TEST"
            }
        }
        stage('Integration TEST') {
            steps {
                echo "Integration TEST"
            }
        }
    }
    post {
        always {
            echo "running job status"
        }
        success {
            echo "successfully executed"
        }
        failure {
            echo "job failed"
        }
    }
}
