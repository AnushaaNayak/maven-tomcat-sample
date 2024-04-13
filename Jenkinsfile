 pipeline {    
    agent any 
    
    tools {
        jdk 'jdk17'
        maven 'maven3'
    }

    stages {
      
        stage('Maven Compile') {
            steps {
            sh  "mvn compile"
            }
        }
        
        stage('Tests') {
            steps {
                sh "mvn test"
            }
        }
       
        stage('Build') {
            steps {
                sh "mvn package"
            }
        }
    }
}
