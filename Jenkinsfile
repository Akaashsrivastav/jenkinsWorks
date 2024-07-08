pipeline {
    agent any

    environment {
        // Define any environment variables here
        NODE_ENV = 'development'
    }

    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from the repository
                git 'https://github.com/acemilyalcin/sample-node-project.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                // Install project dependencies
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                // Run the build script
                sh 'npm run build'
            }
        }

        stage('Test') {
            steps {
                // Run tests
                sh 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                // Deploy the application
                // Adjust this step based on your deployment process
                sh './deploy.sh'
            }
        }
    }

    post {
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
