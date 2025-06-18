pipeline {
    agent any
    stages {
        stage('Configure') {
            steps {
                sh 'cmake -S . -B build'
            }
        }
        stage('Build') {
            steps {
                sh 'cmake --build build'
            }
        }
        stage('Test') {
            steps {
                sh 'cd build && ctest --output-on-failure'
            }
        }
    }
}
