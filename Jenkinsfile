pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Fetch the latest code from GitHub master branch
                git branch: 'master', url: 'https://github.com/abhijasp/demojenkins.git'
            }
        }
        stage('Build') {
            steps {
                // Add your build steps here, e.g., Maven, npm, etc.
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                // Add test steps here
                echo 'Running tests...'
            }
        }
        stage('Deploy') {
            steps {
                // Add deploy steps here
                echo 'Deploying...'
            }
        }
    }

    post {
        always {
            // Actions to take always after build (e.g., clean up, notify)
            echo 'Clean up or notify...'
        }
    }
}
