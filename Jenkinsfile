
pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Alfiya-git/app2.git'
            }
        }

        stage('Deploy') {
            steps {
                script {
                     sh "docker run -itd -p 80:8084 stacksimplify/kube-nginxapp1:1.0.0"

                    }
                }
            }
        }
    }
