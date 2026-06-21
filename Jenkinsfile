pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Fetching code from GitHub...'
            }
        }

        stage('Build') {
            steps {
                echo 'Running build script...'
                sh 'chmod +x app.sh'
                sh './app.sh'
            }
        }

    }

    post {
        success {
            echo 'Build completed successfully'
        }
        failure {
            echo 'Build failed'
        }
    }
}
