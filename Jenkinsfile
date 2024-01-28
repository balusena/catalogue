pipeline {
    agent {
        node { label 'workstation' }
    }

    stages {
        stage('Build') {
            steps {
                sh 'npm install'
                // sh 'npm test'
            }
        }

        stage('Unit Tests') {
            steps {
                echo 'Unit Tests'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'sonar'
              // sh 'sudo sonar-scanner -Dsonar.host.url=http://172.31.40.52:9000 -Dsonar.login=admin -Dsonar.password=admin123 -Dsonar.projectKey=catalogue'
            }
        }

        stage('Security Scans') {
            steps {
                echo 'Security Scans'
            }
        }

        stage('Publish Artifact') {
            steps {
                echo 'Publish Artifacts'
            }
        }
    }
}
