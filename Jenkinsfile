pipeline {
    agent any
    stages {
        stage ('Echo script'){
            steps {
                script {
                    load 'echo.groovy'
                    echo '${rootDir}'
                }
            }
            post {
                always {
                    script {
                        echo 'stage execution finished'
                    }
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
