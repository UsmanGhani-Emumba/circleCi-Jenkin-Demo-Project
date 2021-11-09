
pipeline {
    agent {label "linux"}
    stages {
        stage("build"){
            steps {
                sh """
                  docker build -t hello_there
                """
            }
        }
        stage("test"){
            steps {
                npm run main.js
            }
        }
    }
}