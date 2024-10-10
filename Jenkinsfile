pipeline {
    agent any
    tools {
        jdk 'jdk21'
        maven 'Maven 3.9.9'
    }
    environment {
        WAR_FILE = '/target/roshambo.war'
        TOMCAT_URL = 'http://localhost:8081/'
        TOMCAT_USER = 'sarah'
        TOMCAT_PASSWORD = 'sarah232464'
    }
    stages {
        stage('Clean Project') {
            steps {
                bat 'mvn clean'
            }
        }
        stage('Build Project') {
            steps {
                bat 'mvn package'
            }
        }
    }
}
