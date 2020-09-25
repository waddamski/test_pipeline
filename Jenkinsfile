pipeline {
    agent { docker { image 'python:3.6.5' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
        stage('steps') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps work too"
                    ls -lah
                '''
            }
        }
    }
}

