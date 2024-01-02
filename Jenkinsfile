
pipeline {
    agent any 
    stages {
        stage ('build') {
        steps {
            echo "building the car service"
        }
        }
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
                       // error "simulating error during fortify"
                    }
                }
                stage('checkmarkscan') {
                    steps {
                        echo "executing checkmarkscan"
                        sleep 10
                    }
                }
            }
            stage ('deploy to dev') {
             steps {
            echo "deploying carty service to dev"
              }
            }
             stage ('deploy to test') {
             steps {
            echo "deploying carty service to test"
              }
            }
        }
    }
}
