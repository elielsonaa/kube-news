pipeline{
    agent any

    stages {
        stage ('Build Docker Image'){
            steps {
                script {
                    dockerapp = docker.build("undercrazy/kube-news:${end.BUILD_ID}",'-f ./src/Dockerfile ./src')
                }

            }
        }
    }
}