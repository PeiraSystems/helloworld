pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'ls'
                sh 'docker info'
                sh 'docker build -t dgencare/helloword:${BUILD_NUMBER} .'
                sh 'docker tag dgencare/helloword:${BUILD_NUMBER} dgencare/helloword:latest'
                sh 'docker images'
            }
        }
    }
}