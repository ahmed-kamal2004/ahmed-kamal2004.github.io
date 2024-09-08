pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
              sh 'ls -l'
              sh 'python3'
            }
        }
        stage('Test') { 
            steps {
                sh 'curl localhost:8080'
                sh 'curl localhost:80'
            }
        }
        stage('Deploy') { 
            steps {
               sh 'docker ps'
               sh 'aws sts get-caller-identity'
            }
        }
    }
}
