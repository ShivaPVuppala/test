pipeline {
    agent any
    // stages {
    //     stage('Build') {
    //         steps {
    //             echo 'Building...'
    //             sh 'mvn clean install'
    //         }
    //     }
    //     stage('Test') {
    //         steps {
    //             echo 'Testing...'
    //             sh 'sonar-scanner'
    //         }
    //     }
    //     stage('Deploy') {
    //         steps {
    //             echo 'Deploying...'
    //             sh 'jfrog rt upload'
    //         }
    //     }
        
    // }
    stages {
        stage('Build') {
            steps {
                sh 'javac HelloWorld.java'
            }
        }
        stage('Run') {
            steps {
                sh 'java HelloWorld'
            }
        }
    }
}
