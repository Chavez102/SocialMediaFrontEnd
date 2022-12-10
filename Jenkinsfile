pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        echo 'Building..'
          sh 'npm install --verbose'
        } 
      }
    
    stage('Test') {
      steps {
        echo 'Testing..'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
        sh 'npm start'  
      }
    }
  }
}
