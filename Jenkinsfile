pipeline {
    agent any
    stages {
        stage('build') {
            steps {
            dockerImage = docker.build imagename
            }
        }
    }
}
