
node{
    checkout scm
    stage('Build') {
        docker.image('node:14-alpine').inside('usmdemoproject') {
            sh 'npm --version'
        }
    }
}