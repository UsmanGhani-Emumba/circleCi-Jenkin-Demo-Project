
pipeline {
    agent any
    stages {
        stage('print username') {
            steps {
                echo "username = ${u}"
            }
        }

        stage('print password') {
            steps {
                echo "password = ${adminPassword}"
            }
        }
    }
}
