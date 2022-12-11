pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        echo 'Building..'
        sh 'ls'
          sh 'npx npm@6 install --verbose'
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
        sh 'ls'
        sh 'nohup ng serve &'  
      }
    }
  }
}
