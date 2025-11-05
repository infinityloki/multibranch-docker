pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'docker build -t image2 .'
            }
        }
        stage ("Deploy") {
            steps {
                sh 'docker run -itd --name bus-app -p 2222:80 rajkumar222/paytm:bus'
            }
        }
    }
}
