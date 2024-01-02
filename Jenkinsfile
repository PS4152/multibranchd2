pipeline {
    agent any
    environment {
        DEPLOY_TO = 'productions'
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
            stage ('pro') {
                when {
                    allOf {
                        branch 'production'
                        environment name: 'DEPLOY_TO', value: 'production'
                    }
                }
                steps {
                    echo "depoying to production"
                }
            }
        }
}
