pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/vishalsandhan/Jenkins-daily-task-5.git'
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
