pipeline {
  agent {
    docker {
      image 'maven: 3.6.3-jdk-11'
    }

  }
  stages {
    stage('ci') {
      agent any
      steps {
        sh 'echo "Starting ci"'
        sh 'mvn clean install'
        sh 'Echo "Build done"'
      }
    }

  }
}