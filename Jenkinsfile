pipeline {
  agent any
    stages {
      stage('init') {
        steps {
            sh 'eval $(docker-machine env default --shell bash)'
            echo 'Hello World'
        }
      }
      stage('build') {
        agent { docker 'maven:3.3.3' }
        steps {
          sh 'mvn --version'
        }
      }
    }
}
