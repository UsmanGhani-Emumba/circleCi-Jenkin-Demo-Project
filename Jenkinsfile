
pipeline {
    agent {label "windows"}
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