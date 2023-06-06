pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/carlo-santos-oc/is491freestylejenkins.git'
      }
    }
     
    stage('Build') {
      steps {
        bat 'npm install'
         bat '<<Build Command>>'
      }
    }  
    
            
    stage('Test') {
      steps {
        bat 'node test'
      }
    }
  }
}