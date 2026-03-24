pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'echo "Building project..."'
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
                sh 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploying application..."'
            }
        }
    }
}