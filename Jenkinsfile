pipeline {
    agent any 
    stages {
        stage ('stages running in parallel') {
            parallel {
                stage ('sonarscan') {
                    steps {
                        echo "executing sonar scan"
                        sleep 10
                    }
                }
                stage ('fortifyscan') {
                    steps {
                        echo "executing fortify scan"
                        sleep 10
                    }
                }
                stage('checkmarkscan') {
                    steps {
                        echo "executing checkmarkscan"
                        sleep 10
                    }
                }
            }
        }
    }
}
