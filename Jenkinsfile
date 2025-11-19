pipeline {

    agent { // where should this job be running on ?
        label 'java-slave'
    }
    stages {
        stage ('hostname') { // added a stage
            steps {
                sh 'hostname -i'
            }
        }
        stage('NewStage') { // added a new stage
            steps {
                echo "Welcome to pipelines" // simple echo command
            }  
        }
    }
}
