pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Stage 1: Build'
                echo 'Task: Compiling and packaging the application using Maven.'
                echo 'Tool: Maven'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Task: Running unit tests with JUnit and integration tests with Selenium.'
                echo 'Tools: JUnit (unit tests), Selenium (integration tests)'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Task: Analysing code quality and ensuring it meets industry standards.'
                echo 'Tool: Checkstyle integrated via Jenkins plugin'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Task: Scanning code for known vulnerabilities and security issues.'
                echo 'Tool: OWASP Dependency-Check'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Task: Deploying the application to a staging AWS EC2 instance.'
                echo 'Tool: AWS CLI / SSH deployment scripts'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Task: Running integration tests on the staging server to verify production-like behaviour.'
                echo 'Tool: Selenium / Postman'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Task: Deploying the verified application to the production AWS EC2 instance.'
                echo 'Tool: AWS CLI / SSH deployment scripts'
            }
        }

    }
}
