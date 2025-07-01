pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                echo 'Cloning repo...'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'chmod +x build.sh && ./build.sh'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo "Dummy test passed ✅"'
            }
        }
    }
}
