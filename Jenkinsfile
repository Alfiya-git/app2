
pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Alfiya-git/app2.git'
            }
        }

        stage('Deploy Kube') {
            steps {
                script {
                     sh "kubectl apply -f /app2"

                    }
                }
            }
        }
    }
