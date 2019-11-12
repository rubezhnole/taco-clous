stage('Initialize'){
    def dockerHome = tool 'myDocker'
    env.PATH = "${dockerHome}/bin:${env.PATH}"
}

pipeline {
  agent {
    docker {
      image 'maven:3.3.3'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'mvn --version'
      }
    }

  }
}