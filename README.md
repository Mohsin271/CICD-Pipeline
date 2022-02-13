pipeline {
    agent any
    stages {
        stage('Stage #1 Source') {
            steps {
                echo 'Hello World'
                sleep 10
                echo 'This is the First Stage'
            }
        }
        stage('Stage #2 Build') {
            steps {
                echo 'This is the Second Stage'
            }
        }
        stage('Stage #3 Test') {
            steps {
                echo 'This is the Third Stage'
            }
        }
        stage('Stage #4 Deploy') {
            steps {
                echo 'This is the Forth Stage'
            }
        }
    }
}
