pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'docker build -t image3 .'
            }
        }
        stage ("Deploy") {
            steps {
                sh 'docker run -itd --name movie-app -p 3333:80 rajkumar222/paytm:movie'
            }
        }
    }
}
