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
                bat 'javac TimestampPrinter\\src\\main\\java\\TimestampPrinter.java'
            }
        }
        stage('Run') {
            steps {
                bat 'java -cp TimestampPrinter\\src\\main\\java TimestampPrinter'
            }
        }
    }
}