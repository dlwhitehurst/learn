pipeline {
  sh 'docker-machine create -d virtualbox default'
  agent { docker 'maven:3.3.3' }
    stages {
      stage('build') {
        steps {
          sh 'mvn --version'
        }
      }
    }
}
