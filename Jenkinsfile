pipeline {
  agent any
  stages {
    stage('ci') {
      steps {
        sh 'echo "Starting ci"'
        sh 'mvn clean install'
        sh 'Echo "Build done"'
      }
    }

  }
}