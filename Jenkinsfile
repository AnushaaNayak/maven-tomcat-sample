 pipeline {     
    agent {
     label 'slave-1'
    } 
    
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
