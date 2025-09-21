pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/<your-username>/simple-cicd-windows.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project on Windows...'
                bat 'echo Build Step Running...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'echo Tests executed successfully!'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                bat 'hello.cmd'
            }
        }
    }
}

