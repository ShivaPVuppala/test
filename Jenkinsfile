pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'mvn clean install'
            }
        }
        stage('SonarQube') {
            steps {
                echo 'Running Sonarqube...'
                sh 'sonar-scanner'
            }
        }
        stage('Artifactory') {
            steps {
                echo 'Uploading artifacts to Artifactory...'
                sh 'jfrog rt upload'
            }
        }
    }
}
