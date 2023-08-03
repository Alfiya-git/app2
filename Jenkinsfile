
pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Alfiya-git/app2.git'
            }
        }

        stage('Deploy Docker Container') {
            steps {
                script {
                     sh "docker run -itd -p 81:8083 stacksimplify/kube-nginxapp2:1.0.0"

                    }
                }
            }
        }
    }
