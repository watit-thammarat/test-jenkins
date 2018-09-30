pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Cloning Git') {
      steps {
        git 'https://github.com/watit-thammarat/test-jenkins'
      }
    }
        
    stage('Install dependencies') {
      steps {
        sh 'npm install'
        sh 'npm run bowerInstall'
      }
    }
     
    stage('Test') {
      steps {
         sh 'npm test'
      }
    }      
  }
}