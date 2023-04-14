pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'mvn clean'
        sh 'mvn build'
        withMaven(jdk: 'JDK 17', publisherStrategy: 'implicit')
      }
    }

  }
}