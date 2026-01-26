pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/kirank02072002-boop/jenkins-aws-ci-cd.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t demo-app .'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                docker stop demo-app || true
                docker rm demo-app || true

                docker run -d \
                  --name demo-app \
                  -p 8081:80 \
                  demo-app
                '''
            }
        }
    }
}
