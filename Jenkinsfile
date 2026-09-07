pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application using Maven: compiling source code and packaging into a deployable artifact.'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Running unit tests with JUnit to verify individual components, and integration tests with Selenium to confirm components work together correctly.'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Analysing code quality and maintainability using SonarQube to ensure the codebase meets industry standards.'
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Scanning the codebase for known vulnerabilities using OWASP Dependency-Check.'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Deploying the packaged application to a staging AWS EC2 instance for pre-production testing.'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Running integration tests against the staging environment using Postman to confirm production-like behaviour.'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Deploying the verified application to the production AWS EC2 instance, making it live for end users.'
            }
        }
    }
}
