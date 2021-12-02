
def checkOs(){
    if (isUnix()) {
      sh 'npm run main'
    }
    else {
        sh 'npm run test'
    }
}
pipeline {
    agent any
    stages {
        stage("build"){
            steps {
                echo 'Building the project'
            }
        }
        stage("test"){
            steps {
                echo 'Testing the project'
            }
        }
        stage("check os"){
            steps{
                checkOs()
            }
        }
    }
}