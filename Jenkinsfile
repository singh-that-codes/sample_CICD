pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Step 1: Checkout the source code from the repository
                git 'https://github.com/yourusername/your-repo.git'
            }
        }
        stage('Build') {
            steps {
                // Step 2: Install dependencies and build the project
                sh 'npm install'
                sh 'npm run build'
            }
        }
        stage('Test') {
            steps {
                // Step 3: Run tests
                sh 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                // Step 4: Deploy the application (Replace with your deployment commands)
                // For example, deploying to a web server or container
                sh 'npm run deploy'
            }
        }
    }
}

