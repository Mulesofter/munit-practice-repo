pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Jenkins loaded the pipeline.'
            }
        }
        stage('Verify Java and Maven') {
            steps {
                bat 'java -version'
                bat 'call "C:/Program Files/Maven/apache-maven-3.9.6/bin/mvn.cmd" -version'
            }
        }
    }
}
