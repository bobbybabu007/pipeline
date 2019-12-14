pipeline {
    agent any;
    stages {
        stage('Set Up') {
           steps {
               cleanWs();
               sh 'echo setting up my workspace'
           }
        }
        stage('Checkout SCM') {
            steps {
                sh 'triggering a build using web hook'
                checkout scm
            }
        }
        stage('Compile Code') {
            steps {
                sh 'chmod +x app.sh'
            }
        }
        stage('Testing ') {
            steps {
                sh 'sh app.sh'
            }
        }
    }
}
