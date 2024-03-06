pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    echo 'Compiling the C++ file...'
                    sh "g++ -o PES1UG21CS342-1 PES1UG21CS342.cpp"
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    echo 'Running the C++ program...'
                    sh "./PES1UG21CS342-1"
                }
            }
        }

        stage('Deploy') {
            steps {
                 echhho 'Deployment stage'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed!'
        }
    }
}
