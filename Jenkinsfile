pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
               git branch: 'main', url: 'https://github.com/shreekanth7899/Jenkins-Deployment.git'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Testing'
            }
        }
    }
}
