pipeline {
    agent any 
    stages {
        stage('Clean the build') { 
            steps {
                msh "mvn clean"
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test"
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package"
            }
        }
    }
}
