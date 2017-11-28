pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
            def app = docker.build "dgencare/helloword:${env.BUILD_NUMBER}"
        }
    }
}