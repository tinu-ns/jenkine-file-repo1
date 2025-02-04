pipeline {
    agent any

    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', credentialsId: 'git-credential', url: 'https://github.com/tinu-ns/jenkine-file-repo1.git'
            }
        }
        stage('Maven build') {
            steps {
                sh 'mvn clean package'
            }
        } 
   }
}


