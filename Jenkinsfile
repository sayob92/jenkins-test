pipeline {
    agent any 
    stages {
        stage('Build application') { 
            steps { 
                bat 'mvn clean install'
            }
        }
      
        stage('Deploy application to cloudhub') { 
            steps {
                bat 'mvn package deploy -DmuleDeploy'
            }
        }
    }
}