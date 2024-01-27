pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Your build steps here
                echo 'Building the project...'
            }
        }

        stage('Deploy to Development') {
            when {
                branch 'development'
            }
            steps {
                // Deployment steps for the development environment
                echo 'Deploying to the development environment...'
            }
        }

        stage('Deploy to Test') {
            when {
                branch 'test'
            }
            steps {
                // Deployment steps for the test environment
                echo 'Deploying to the test environment...'
            }
        }

        stage('Deploy to Production') {
            when {
                branch 'master'
            }
            steps {
                // Deployment steps for the production environment
                echo 'Deploying to the production environment...'
            }
        }
    }
}
