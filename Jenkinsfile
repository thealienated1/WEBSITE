pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/thealienated1/WEBSITE.git'
            }
        }

        stage('Copy to Test Server') {
            steps {
                sh 'scp -r . ubuntu@172.31.82.99:/path/to/directory'
            }
        }
    }
}
