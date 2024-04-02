pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                git 'https://github.com/shreekanth7899/Jenkins-Deployment.git'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
