pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from GitHub
                git 'https://github.com/your-username/java-timestamp-ci.git'
            }
        }
        stage('Build') {
            steps {
                // Compile the Java program
                sh 'javac TimestampPrinter.java'
            }
        }
        stage('Run') {
            steps {
                // Execute the Java program
                sh 'java TimestampPrinter'
            }
        }
    }
}
