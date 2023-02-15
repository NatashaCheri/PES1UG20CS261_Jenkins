pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ -o program_exec program.cpp'
            }
        }
        stage('Test') {
            steps {
                sh './program_exec'
            }
        }
        stage('Deploy') {
            steps {
            }
        }
    }

    post {
        
        failure {
            echo 'Pipeline failed.'
        }
    }
}
