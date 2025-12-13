pipeline {
    agent any

    stages {
        stage('Run Python') {
            steps {
                script {
                    docker.image('python:3.14.2-alpine3.23').inside('--workdir /workspace') {
                        sh 'python --version'
                    }
                }
            }
        }
    }
}
