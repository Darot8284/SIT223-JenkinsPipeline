pipeline {
    agent any

    triggers {
        pollSCM('H/2 * * * *')   // Checks GitHub every 2 minutes
    }

    stages {

        stage('Build') {
            steps {
                echo 'Stage 1: Build'
                echo 'Task: Compile and package application'
                echo 'Tool: Maven'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Task: Execute unit and integration tests'
                echo 'Tool: JUnit'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Task: Analyse code quality and standards'
                echo 'Tool: SonarQube'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Task: Scan for security vulnerabilities'
                echo 'Tool: OWASP Dependency-Check'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Task: Deploy application to staging environment'
                echo 'Tool: AWS EC2'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Task: Validate application in staging environment'
                echo 'Tool: Selenium'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Task: Deploy application to production environment'
                echo 'Tool: AWS EC2'
            }
        }
    }
}
