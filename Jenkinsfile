pipeline {
    agent any

    stages {
        stage('Git') {
            steps {
                git 'https://github.com/somaanath/BoardgameListingWebApp'
            }
        }
         stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
         stage('Test') {
            steps {
                 sh 'mvn test'
            }
        }
         stage('Package'){
            steps {
                 sh 'mvn clean package'
            }
        }
        stage('Docker'){
            steps {
                 echo 'Docker'
            }
        }
    }
}
