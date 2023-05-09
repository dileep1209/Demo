pipeline {

    agent any

    tools {

        maven "maven"
    }

    
    stages {
        stage('Build Maven') {
            steps{
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/dileep1209/Demo.git']])
                sh "mvn clean package"
                
            }
        }
    }
    
}
