
pipeline {
    agent any
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
                node main.js
            }
        }
    }
}