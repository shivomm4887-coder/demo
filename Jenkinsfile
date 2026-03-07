pipeline {
    agent any

    stages {
        stage('CheckOut') {
            steps {
                git branch: 'main', url: 'https://github.com/shivomm4887-coder/demo.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Build in progress.....'
                bat 'javac Hello.java'
            }
        }
        stage('Execute') {
            steps {
                echo 'Executing....'
                bat 'java Hello'
            }
        }
    }
}
