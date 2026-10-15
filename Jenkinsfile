
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Source code checked out from GitHub.'
            }
        }

        stage('Verify Java and Maven') {
            steps {
                bat 'java -version'
                bat 'call "C:/Program Files/Maven/apache-maven-3.9.6/bin/mvn.cmd" -version'
            }
        }

        stage('Run MUnit Tests') {
            steps {
                bat 'call "C:/Program Files/Maven/apache-maven-3.9.6/bin/mvn.cmd" clean test'
            }
        }
    }
}
