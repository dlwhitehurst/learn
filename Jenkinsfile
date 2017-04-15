pipeline {
  agent any
  stages {
        stage('Example') {
            steps {
                sh 'eval $(docker-machine env default --shell bash)'
                echo 'Hello World'
            }
        }
    }
  agent { docker 'maven:3.3.3' }
    stages {
      stage('build') {
        steps {
          sh 'mvn --version'
        }
      }
    }
}
