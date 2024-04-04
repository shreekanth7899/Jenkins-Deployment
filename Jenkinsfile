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
                sh 'scp -r /etc/nginx/site-available* shreekanth@127.0.0.1:/etc/nginx/site-available'
                sh 'scp -r /var/www/jenkins-d/Jenkins-Deployment* shreekanth@127.0.0.1:/var/www/jenkins-d/Jenkins-Deployment'
            }
        }
       stage('Restart Nginx') {
            steps {
                sh 'ssh shreekanth@127.0.0.1 sudo systemctl restart nginx'
            }
        }
    }
}
