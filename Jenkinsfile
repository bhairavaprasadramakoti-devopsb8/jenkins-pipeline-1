pipeline {
    agent { // where should this job be running on ?
        label 'java-slave'
    }
    stages {
        stage ('Build') {
            steps {
                echo "This is a build stage"
            }
        }
        stage('groovycodestage') {
            steps {
                script {
                    // define a variable
                    def course = "k8s"

                    // if condition
                    if (course == "k8s") {
                        println("Thanks for enrolling to k8s course")
                    } else {
                        println("Do enroll to k8s")
                    }
                }
            }
        }
    }
}   
