pipeline {
    agent { docker { image 'python:3.10.1-alpine' } }
     stage('Initialize'){
        def dockerHome = tool 'myDocker'
        env.PATH = "${dockerHome}/bin:${env.PATH}"
    }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
}
