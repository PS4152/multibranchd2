pipeline {
    agent any
    stages {
        stage ("build") {
            steps {
                echo "welcome to build stage"
            }
        }
        stage ('deploy to dev') {
            steps {
                echo "deploying to dev environment"
            }
        }
        stage ('deploy to stage') {
            when {
                expression {
                    // stagr should execute with either production branch or staging branch
                    BRANCH_NAME ==~ /(production|staging)/
                }
            }
            steps {
                echo "deploying to stage environment"
            }
        }

    }
}
