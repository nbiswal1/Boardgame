pipeline {
    agent any
    
    tools {
        jdk 'Java 17'
        maven 'Maven 3.9'
    }

    stages {
        stage('Verify Tools') {
            steps {
                sh 'java -version'
                sh 'mvn -version'
            }
        }

        stage('mvn validate') {
            steps {
                sh 'mvn validate'
            }
        }

        stage('mvn compile') {
            steps {
                sh 'mvn compile'
            }
        }

        stage('mvn test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('mvn package') {
            steps {
                sh 'mvn package'
            }
        }
        stage('mvn install') {
            steps {
                sh 'mvn install'
            }
        }

        stage('mvn deploy') {
            steps {
                sh 'mvn deploy'
            }
        }
    }
}
