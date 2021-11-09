
// node('docker') {
//     checkout scm
//     stage('Build') {
//         docker.image('node:14-alpine').inside {
//             sh 'npm --version'
//             echo "Hello"
//         }
//     }
// }

pipeline {
    agent any
    stages {
        stage ("build"){
            steps {
                echo "Building the project"
            }
        }
        stage ("test"){
            steps {
                echo "Testing the project"
            }
        }
    }
}