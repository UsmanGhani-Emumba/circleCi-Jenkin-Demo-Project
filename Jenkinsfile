
node{
    checkout scm
    stage('Build') {
        docker.image('node:14-alpine').inside("E:\circleCi_Jenkins_Demo\usmdemoproject"){
            sh 'npm --version'
        }
    }
}