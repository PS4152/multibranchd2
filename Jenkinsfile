pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('build') {
            steps {
                echo "welocme to build stage"
            }
        }
            stage ('deploy to dev') {
                steps {
                    echo "deploying to dev stage"
                }
            }
            stage {
                when {
                    allOf {
                        branch 'production'
                        environment name = 'DEPLOY_TO', value: production
                    }
                }
            }
        }
}
