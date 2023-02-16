pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ -o file_exec file.cpp'
            }
        }
        stage('Test') {
            steps {
                sh './file_exec'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployment successful for PES1UG20CS263 pipeline'
            }
        }
    }

    post {
        
        failure {
            echo 'Pipeline failed.'
        }
    }
}
