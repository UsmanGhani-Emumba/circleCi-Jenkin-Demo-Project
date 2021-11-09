
pipeline {
    agent {label "linux"}
    stages {
        stage("build"){
            steps {
                echo "My first demo project"
            }
        }
        stage("test"){
            steps {
                npm run main.js
            }
        }
    }
}