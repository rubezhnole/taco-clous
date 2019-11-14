pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "This is my first step"
            }
        }
        stage('Test') {
            steps {
                './gradlew test'
            }
        }
        stage('Deploy') {
            steps {
                echo "This is my Deploy step"
            }
        }
    }
}