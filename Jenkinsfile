pipeline {
    //agent any
    agent { docker { image "maven:3.6.3"} }

    stages {
        stage('Build') {
            steps {
                sh "mvn --version"
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
