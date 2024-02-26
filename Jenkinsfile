pipeline {
    agent any{
        node{
            label "linux && java11"
        }
    }
    
    stages {
        stage('Build'){
            steps {
                echo("Start Build")
                sh("./mvnw clean compile test-compile")
                echo("Finish Build")
            }
        }
        stage('Test'){
            steps {
                echo("test Build")
                sh("./mvnw test")
                echo("test Build")
            }
        }
        stage('Deploy'){
            steps {
                echo("Hello deploy 1")
                sleep(5)
                echo("Hello deploy 2")
                echo("Hello deploy 3")
            }
        }
    }

    post {
        always {
            echo "i will always hello again"
        }
        success {
            echo "yes, success!"
        }
        failure {
            echo "oh no, failure!"
        }
        cleanup {
            echo "dont care success or error"
        }
    }
}