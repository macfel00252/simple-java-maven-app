pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn -B -DSkipTests clean package'
      }
    }
  }
}