pipeline {
    agent any

    stages {
        stage('Matrix Build') {
            matrix {
                axes {
                    axis {
                        name 'NODE_VERSION'
                        values '14', '16', '18'
                    }
                }
                stages {
                    stage('Install') {
                        steps {
                            sh 'npm install'
                        }
                    }
                    stage('Test') {
                        steps {
                            sh 'npm test'
                        }
                    }
                }
            }
        }
    }
}
