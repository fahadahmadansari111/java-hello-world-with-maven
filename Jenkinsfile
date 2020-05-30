pipeline {
  agent any
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
}