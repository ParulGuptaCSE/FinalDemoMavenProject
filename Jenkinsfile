pipeline {
    agent any
    environment {
        PATH = "/Users/parulgupta/Downloads/apache-maven-3.6.3/bin:$PATH"
    }
    stages {
        stage('Clone and clean') { 
            steps {
                sh "mvn clean"
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test"
            }
        }
        stage('Package') { 
            steps {
                sh "mvn package"
            }
        }
    }
}
