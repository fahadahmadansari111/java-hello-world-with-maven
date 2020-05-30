pipeline {
  agent any
  stages {
    stage('Initialize')
    {
        def dockerHome = tool 'MyDocker'
        def mavenHome  = tool 'MyMaven'
        env.PATH = "${dockerHome}/bin:${mavenHome}/bin:${env.PATH}"
    }
    stage('ci') {
      steps {
        sh 'echo "Starting ci"'
        sh 'mvn clean install'
        sh 'Echo "Build done"'
      }
    }

  }
}
