pipeline {
    agent any
    stages {
        stage('build') {
            steps {
		sh 'sudo docker build --name microblog:test .'
		sh 'sudo docker run --name microblog -d -p 8000:5000 --rm microblog:test'
            }
        }
    }
}
