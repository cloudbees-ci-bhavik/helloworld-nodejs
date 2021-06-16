pipeline {
  agent none
  stages {
    stage('Test') {
      agent { label 'nodejs-app' }
      steps {
        sh 'java -version'
        container('nodejs') {
          sh 'node --version'
          echo 'Hello World!'
        }
      }
    }
  }
}
