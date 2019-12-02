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
                gradle('test')
                gradle {
                    tasks('clean')
                    tasks('test')
                    switches('--info')
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