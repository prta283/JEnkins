pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning the repo...'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                stage('Info') {
    steps {
        sh 'uname -a'
    }
}

            }
        }
    }
}
