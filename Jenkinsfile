pipeline {
  agent { docker 'maven:3.3.3' }
    stages {
      stage('init') {
        steps {
            sh 'eval $(docker-machine env default --shell bash)'
            echo 'Hello World'
        }
      }
      stage('build') {
        steps {
          sh 'mvn --version'
        }
      }
    }
}
