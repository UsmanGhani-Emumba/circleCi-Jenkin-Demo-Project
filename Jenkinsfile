
pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            steps {
                  echo 'building the applications'
            }
        }
        stage('Test') {
                    steps {
                        echo 'testing the applications'
                    }
                }
    }
}