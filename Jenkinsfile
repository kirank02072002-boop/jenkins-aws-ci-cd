pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'docker build -t demo-app .'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                  docker stop web || true
                  docker rm web || true
                  docker run -d -p 80:80 --name web demo-app
                '''
            }
        }
    }
}
