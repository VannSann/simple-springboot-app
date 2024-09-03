pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Retrieve the source code from version control
                checkout scm
            }
        }

        stage('Build and Package') {
            steps {
                script {
                    // Build and package the Spring Boot application using Maven
                    sh 'mvn clean package'
                }
            }
        }
    }
}
