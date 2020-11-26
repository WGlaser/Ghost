pipeline {
  agent any
    
  tools {
      nodejs "node"
      
  }
    
  stages {
    stage('Build') {
      steps {
       git 'https://github.com/WGlaser/Ghost.git'
          
       sh 'rm -rf ./node_modules'
        sh 'export PATH="/usr/local/bin:$PATH"' 
       sh 'npm cache clean --force'
    
       sh 'npm install yarn -g'
       sh 'npm install -g'
       sh 'npm install ghost-cli -g'
       
       
      }
    }  
    
          
    stage('Test') {
      steps {
       sh 'npm test'
      }
    }
  }
}
