pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                echo 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'File used for example test: '
                echo './jenkins/scripts/test.sh'
            }
        }
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }            
    }
}

