pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Running Build Script'
                sh 'chmod +x app.sh'
                sh './app.sh'
            }
        }

        stage('Test') {
            steps {
                echo 'Running Test Script'
                sh 'chmod +x test.sh'
                sh './test.sh'
            }
        }

    }
}
