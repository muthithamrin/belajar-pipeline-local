pipeline {
    agent{
        node{
            label "linux && java11"
        }
    }
    
    stages {
        stage('Hello'){
            steps {
                echo("Hello Pipeline")
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