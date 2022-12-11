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
        sh 'pwd'
        sh 'JENKINS_NODE_COOKIE=dontKillMe nohup ng serve --host=0.0.0.0 > ~/mylogs.out 2>&1 &'
      }
    }
  }
}
