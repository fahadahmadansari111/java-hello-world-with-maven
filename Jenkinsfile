pipeline {
  agent {
    docker {
      image 'maven:3.6.3-jdk-11'
    }

  }
  stages {
    stage('Initialize') {
      agent any
      environment {
        dockerHome = 'myDocker'
        mavenHome = 'myMaven'
        PATH = '${dockerHome}/bin:${mavenHome}/bin:${env.PATH}'
      }
      steps {
        sh 'echo "Done"'
      }
    }

  }
  environment {
    myDocker = 'myDocker'
    PATH = '${myDocker}/bin:${env.PATH}'
  }
}