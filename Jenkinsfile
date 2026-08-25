pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo '=== Stage 1: Checkout Complete ==='
            }
        }
        stage('Build') {
            steps {
                echo '=== Stage 2: Building Application ==='
                sh 'date'
            }
        }
        stage('Test') {
            steps {
                echo '=== Stage 3: Running Tests ==='
                sh 'pwd && ls -la'
            }
        }
        stage('Deploy') {
            steps {
                echo '=== Stage 4: Deploying App ==='
                echo 'Deployment successful!'
            }
        }
    }
    
    post {
        always {
            echo 'Pipeline execution finished.'
        }
    }
}
