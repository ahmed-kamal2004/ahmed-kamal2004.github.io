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
               sh 'sudo service nginx status'
               sh 'sudo service jenkins status'
            }
        }
        stage('Deploy') { 
            steps {
               sh 'docker ps'
            }
        }
    }
}
