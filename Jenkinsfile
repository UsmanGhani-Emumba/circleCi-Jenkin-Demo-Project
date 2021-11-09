
pipeline {
    agent {
        docker
            { 
                image 'node:14-alpine' 
            }
    }
    stages {
        stage ("build"){
            steps {
                echo 'Building the project'
            }
        }
        stage ("test"){
            steps {
                echo 'Testing the project'
            }
        }
        stage("run"){
            steps {
                sh 'node main.js'
            }
        }
    }
}