pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ hello.cpp'
                build job: 'PES2UG20CS540-1'
            }
        }
        stage('Test') {
            steps {
                sh './a.out'
                echo "Build stage successful"
            }
        }
        stage('Deploy') {
            steps {
                echo "Deployment s
            }
        }
    }
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
