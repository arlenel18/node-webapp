pipeline {
    agent any
    
    stages {
        stage('Build and Run') {
            steps {
                sh 'docker build . -t node-app:latest'
                sh 'docker run -d -p 3000:3000 --name node-app node-app:latest'
            }
        }
    }
}
