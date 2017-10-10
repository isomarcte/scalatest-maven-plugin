pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                mvn clean test-compile
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                mvn verify
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                mvn install
            }
        }
    }
}
