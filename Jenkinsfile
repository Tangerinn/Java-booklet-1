pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Compiling the BinarySearch and BinarySearchTest files...'
                bat 'javac -cp "junit-4.13.2.jar;." BinarySearch.java BinarySearchTest.java'
            }
        }
        stage('Test') {
            steps {
                echo 'Running automated test cases...'
                bat 'java -cp "junit-4.13.2.jar;." org.junit.runner.JUnitCore BinarySearchTest'
            }
        }
    }
}
