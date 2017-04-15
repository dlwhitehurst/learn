pipeline {
  agent any
  sh 'eval $(docker-machine env default --shell bash)'
  agent { docker 'maven:3.3.3' }
    stages {
      stage('build') {
        steps {
          sh 'mvn --version'
        }
      }
    }
}
