
def checkOs() {
    if (isUnix()) {
        sh 'npm run main'
    }
    else {
        sh 'npm run test'
    }
}
pipeline {
    agent any
    parameters {
        choice(name: 'Environment', choices: ['QA', 'Perf', 'UAT'], description: 'Choose an environment')
        choice(name: 'Username', choices: ['nikhilQA', 'nikhilPerf', 'nikhilUAT'], description: 'Choose a username')
        choice(name: 'Password', choices: ['salesforce3', 'salesforce4', 'salesforce5'], description: 'Choose a password')
    }
    stages {
        stage('build') {
            when {
                expression {
                            params.Environment == 'QA' &&
                            params.Username == 'nikhilQA' &&
                            params.Password == 'salesforce3'
                }
            }
            steps {
                echo "environment = ${params.Environment}"
                echo "username = ${params.Username}"
            }
        }
        stage('test') {
            steps {
                echo "${params.Username}" >> config.json
            }
        }
        stage('check os') {
            steps {
                checkOs()
            }
        }
    }
}
