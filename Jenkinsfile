pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from GitHub
                git 'https://github.com/vishalsandhan/Jenkins-daily-task-5'
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
