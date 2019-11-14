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
                if (isUnix()) {
                    sh 'gradle test --info'
                } else {
                    bat 'gradle test --info'
                }
            }
        }
        stage('Deploy') {
            steps {
                echo "This is my Deploy step"
            }
        }
    }
}