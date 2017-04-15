pipeline {
    agent { docker 'maven:3.3.3' }
    stages {
        stage('build') {
            steps {
                timeout(time: 10, unit: 'MINUTES') {
                  sh 'mvn --version'
                }
            }
        }
    }
}
