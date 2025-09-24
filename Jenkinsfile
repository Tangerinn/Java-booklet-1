pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Compiling the BinarySearch and BinarySearchTest files...'
                bat '"C:\\Program Files\\Java\\jdk-21\\bin\\javac" -cp junit-4.13.2.jar:. BinarySearch.java BinarySearchTest.java'
            }
        }
        stage('Test') {
            steps {
                echo 'Running automated test cases...'
                bat '"C:\\Program Files\\Java\\jdk-21\\bin\\java" -cp junit-4.13.2.jar:. org.junit.runner.JUnitCore BinarySearchTest'
            }
        }
    }
}
