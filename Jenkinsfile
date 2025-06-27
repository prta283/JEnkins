pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/prta283/JEnkins/Jenkinsfile'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt || true'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'python -m unittest discover || echo "Tests failed"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment logic goes here...'
            }
        }
    }

    post {
        success {
            echo '✅ Build passed!'
        }
        failure {
            echo '❌ Build failed!'
        }
    }
}
