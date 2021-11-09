
node{
    checkout scm
    stage('Build') {
        docker.image('node:14-alpine').inside('circleCi-Jenkin-Demo-Project') {
            sh 'npm --version'
        }
    }
}