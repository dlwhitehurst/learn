pipeline {
  agent any
    stages {
      stage('build') {
        steps {
            sh 'eval $(docker-machine env default --shell bash)'
            sh 'docker run maven:3.3.3'
            sh 'mvn --version'
            echo 'Hello World'
        }
      }
    }
}
