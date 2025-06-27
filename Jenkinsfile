pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/prta283/JEnkins/Jenkinsfile'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy step (simulated)...'
            }
        }
    }

    post {
        success {
            echo '✅ Build passed and project is ready to deploy.'
        }
        failure {
            echo '❌ Build or tests failed. Check logs.'
        }
    }
}
