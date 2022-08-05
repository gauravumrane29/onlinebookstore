pipeline{
    agent any
    stages{
        stage('scm checkout'){
            steps{
            git "https://github.com/gauravumrane29/onlinebookstore.git"
            }
        }
        stage('Build'){
            steps{
               sh 'mvn clean install'
            }
        }
        stage('Test'){
            steps{
                sh 'mvn test'
            }
        }     
    }
}
