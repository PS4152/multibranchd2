pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('build') {
            steps {
                echo "welcome to build"
            }
        }
        stage ('test') {
            when {
                anyOf {
                    branch  'production'
                    environment name :'DEPLOY_TO', value: 'productions'
                }
            }
            steps {
                echo "deploying to test"
            }
        }
    }
}
