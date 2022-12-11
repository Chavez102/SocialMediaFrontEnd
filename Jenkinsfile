pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        echo 'Building..'
        sh 'ls'
          sh 'npx npm@6 install --verbose'
          sh 'ng build'
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
        sh 'JENKINS_NODE_COOKIE=dontKillMe nohup ng serve &'  
      }
    }
  }
}
