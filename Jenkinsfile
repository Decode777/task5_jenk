pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Decode777/task5_jenk.git'
            }
        }
        stage('Build') {
            steps {
                bat 'javac TimestampPrinter.java'
            }
        }
        stage('Run') {
            steps {
                bat 'java TimestampPrinter'
            }
        }
    }
}