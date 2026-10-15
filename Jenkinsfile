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
                bat 'mvn -version'
            }
        }
    }
}
