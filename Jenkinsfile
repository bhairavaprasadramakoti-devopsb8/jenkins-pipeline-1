pipeline {
    agent {
        label 'java-slave'
    }
    tools {
        maven 'MAVEN_3.9.8' // specify the same Maven installation name configured in Jenkins
    }
    stages {
        stage ('Maven') {
            steps {
                echo "hello, this is maven section"
                sh "mvn --version"
                }
            }
        stage ("SecondStage"){
            // whatever u write under the stage will be taking presedence. 
            tools {
                maven "MAVEN_3.9.6" // specify a different Maven installation for this stage
            }
            steps {
                echo "hello from second stage"
                sh "mvn --version"
            }
        }
    }
}
