pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn -B -DSkipTests clean package'
      }
    }
    stage('Test') {
      steps {
        sh 'mvn test'
        junit 'target/surefire-reports/*.xml'
      }
    }
  }
}