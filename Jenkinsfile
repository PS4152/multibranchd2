pipeline {
    agent any 
    stages {
        stage ('stages running in parallel') {
            failFast true 
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
                        error "simulating error during fortify"
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
