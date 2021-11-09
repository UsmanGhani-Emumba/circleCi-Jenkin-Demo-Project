
node('docker'){
      checkout scm {
          staged ('Build'){
              docker.image('node:14-alpine').inside{
                  sh 'npm --version'
              }
          }
      }
}