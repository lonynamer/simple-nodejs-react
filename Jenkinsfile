pipeline{
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 80:80'
    }
  }
  environment{
    CI = 'true'
  }
  stages{
    stage('Build'){
      steps{
        sh 'npm install'
      }
    }
  }
}
