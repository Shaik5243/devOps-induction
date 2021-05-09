pipeline {
  agent any
    
  tools {nodejs "nodejs"}
    
  stages {

    stage('Install dependencies') {
      steps {
        sh 'npm install -y'
      }
    }
     
    stage('Build') {
      steps {
         sh 'npm run build'
      }
    }  
    stage('Package') {
      steps {
         sh 'ls -lrt'
         sh 'pwd'
         sh 'tar -zcf build.tar.gz build/'
      }
    }    
  }
}
