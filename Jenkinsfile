pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Decode777/task5_jenk.git'
            }
        }
        stage('Build') {
            steps {
                sh 'javac TimestampPrinter.java'
            }
        }
        stage('Run') {
            steps {
                sh 'java TimestampPrinter'
            }
        }
    }
}