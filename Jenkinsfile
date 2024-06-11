pipeline {
    agent any
    environment {
        JAVA_HOME = 'C:\\Program Files\\Java\\jdk-17'
        M2_HOME = 'C:\\Program Files\\Java\\jdk-21'
        PATH = "${env.M2_HOME}\\bin;${env.JAVA_HOME}\\bin;${env.PATH}"
    }
    stages {
        stage('Build') { 
            steps {
                bat 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
