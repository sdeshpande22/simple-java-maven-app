pipeline {
    agent any
    environment {
        JAVA_HOME = 'C:\\Program Files\\Java\\jdk-21'
        MAVEN_HOME = 'C:\\Program Files\\apache-maven-3.9.7'
        PATH = "${env.MAVEN_HOME}\\bin;${env.JAVA_HOME}\\bin;${env.PATH}"
    }
    stages {
        stage('Print Environment Variables') {
            steps {
                bat 'set'
            }
        }
        stage('Verify Maven') {
            steps {
                bat 'mvn -version'
            }
        }
        stage('Build') {
            steps {
                bat 'mvn clean install'
            }
        }
    }
}
