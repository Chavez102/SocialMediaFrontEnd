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
        sh 'JENKINS_NODE_COOKIE=dontKillMe nohup ng serve --host=144.62.209.192 disable-host-check > ~/mylogs.out 2>&1 &'
      }
    }
  }
}
