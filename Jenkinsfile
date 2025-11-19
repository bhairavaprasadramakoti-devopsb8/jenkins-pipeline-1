pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage ('Build') {
            steps {
                echo "Welcome to jenkins pipeline"
                error "this is a failure"
            }
        }
        stage ('Scans') {
            steps {
                echo "Executing Sonar Scans ..."
            }
        }
    }
}
