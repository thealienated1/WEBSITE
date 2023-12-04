pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'test', url: 'https://github.com/thealienated1/WEBSITE.git'
            }
        }

        stage('Copy to Test Server') {
            steps {
                sh 'scp -r . ubuntu@44.204.156.172:/home/ubuntu/jenkins'
            }
        }
    }
}
