pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'develop', url: 'https://github.com/thealienated1/WEBSITE.git'
            }
        }

        stage('Copy to Folder') {
            steps {
                script {
                    sh 'sudo chmod 777 /home/ubuntu/Jenkins'
                    sh 'cp -r * /home/ubuntu/Jenkins'
                }
            }
        }
    }
}
