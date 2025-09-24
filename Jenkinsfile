pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'javac BinarySearch.java'
            }
        }
        stage('Run') {
            steps {
                sh 'java BinarySearch'
            }
        }
    }
}
