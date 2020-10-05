pipeline {
    agent any
    stages {
        stage('compile stage') {
            steps {
                withMaven(maven:'MAVEN'){
                    bat "mvn clean compile"
                }
            }
        }
        stage('testing stage') {
            steps {
                withMaven(maven:'MAVEN'){
                    bat "mvn test"
                }
            }
        }
        stage('Deployement Stage') {
            steps {
                withMaven(maven:'MAVEN'){
                    bat "mvn deploy"
                }
            }
        }
    }
}
