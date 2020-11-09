pipeline {
  environment {
    dockerImage = ''
  }
  agent any
  stages {
    stage('Cloning Git') {
      steps {
        git 'https://github.com/barattar1991/microblog.git'
      }
    }
    stage('Building image') {
      steps{
        script {
	  dockerImage = docker.build registry + ":$BUILD_NUMBER"
          docker.build registry + ":$BUILD_NUMBER"
        }
      }
    }
  }
}
