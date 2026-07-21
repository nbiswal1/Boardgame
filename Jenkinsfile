pipeline {
    // agent {label 'slave-1'}
    agent any
    
    tools {
        maven 'maven 3.9.16'
        jdk 'Java 17'
    }

    stages {     
        stage('Compile') {
            steps {
               sh "mvn compile"
            }
        }
        
        stage('Test') {
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
