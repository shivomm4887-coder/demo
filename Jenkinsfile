pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
               
                git 'https://github.com/shivomm4887-coder/demo.git'
            }
        }

        stage('Publish') {
            steps {
                publishHTML([
                    allowMissing:true,
                    alwaysLinkToLastBuild:false,
                    keepAll:false,
                    reportDir:'.',
                    reportFiles:'index.html',
                    reportName:'My HTML Pipe Page'
                ])
            }
        }
    }
}
