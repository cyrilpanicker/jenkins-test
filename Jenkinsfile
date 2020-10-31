pipeline {
    agent { docker { image 'golang' } }
    stages {
        stage('Build') {
            steps {
                sh 'go version'
                sh 'echo "Hello World"'
            }
        }
        stage('Deploy') {
            steps {
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}
