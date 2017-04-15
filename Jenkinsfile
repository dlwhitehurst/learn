pipeline {
  sh '@FOR /f "tokens=*" %i IN ('docker-machine env') DO @%i'
  agent { docker 'maven:3.3.3' }
    stages {
      stage('build') {
        steps {
          sh 'mvn --version'
        }
      }
    }
}
