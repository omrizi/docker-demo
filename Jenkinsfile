pipeline {
  agent {
    docker {
      image 'node:lts-buster-slim' 
      args '-p 3000:3000'
    }
  }
  stages {
    stage('Project Type Determine'){
      steps{
        sh '''
           pwd
           ls -la
        '''
      }
    }
    stage('Build') {
      steps{
        sh 'npm install'
      }
    }
  }
}
