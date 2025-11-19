pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage ('Build') {
            steps {
                retry(3) {
                    echo "Welcome to jenkins pipeline"
                    error "this is a failure"
                }
            echo "After 3 retries"
            }
        }
        stage ('Scans') {
            steps {
                echo "Executing Sonar Scans ..."
            }
        }
    }
}
