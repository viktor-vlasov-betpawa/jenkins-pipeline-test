pipeline {
    agent any
    stages {
        stage ('Echo script'){
            steps {
                script {
                    load 'echo.groovy'
                }
            }
        }
    }
    post {
        always {
            script {
                echo 'pipeline execution finished'
            }
        }
    }
}
