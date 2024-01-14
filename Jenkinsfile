pipeline {
    agent{
        node{
            label "linux && java11"
        }
    }
    
    stages {
        stage('Build'){
            steps {
                echo("Hello build 1")
                echo("Hello build 2")
                echo("Hello build 3")
            }
            }
            }
        }
        stage('Test'){
            steps { 
                echo("Hello Test 1")
                echo("Hello Test 2")
                echo("Hello Test 3")
            }
        }
        stage('Deploy'){
            steps {
                echo("Hello deploy 1")
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