pipeline {
    agent { docker { image 'golang' } }
    stages {
        stage('init') {
            steps {
                sh 'go version'
            }
        }
        stage('build') {
            steps {
                sh 'go build -o bin/main cmd/builder/main.go'
            }
        }
    }
}
