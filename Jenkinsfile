pipeline {
    agent{
        node{
            label "linux && java11"
        }
    }
    
    stages {
        stage('Build'){
            steps {
                echo("Hello build")
            }
        }
        stage('Test'){
            steps {
                echo("Hello Test")
            }
        }
        stage('Deploy'){
            steps {
                echo("Hello deploy")
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