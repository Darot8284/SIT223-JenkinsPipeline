pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Stage 1: Build - Maven'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: JUnit'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Stage 3: SonarQube'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Stage 4: OWASP Dependency Check'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: AWS EC2 Staging'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Selenium'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: AWS EC2 Production'
            }
        }
    }
}
