pipeline {
    agent any
    stages {
        stage('build') {
            steps {
		   sh "docker build --name microblog:test ."
		   sh "docker run --name microblog -d -p 8000:5000 --rm microblog:test"
            }
        }
    }
}
