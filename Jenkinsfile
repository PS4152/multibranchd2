pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('deploy') {
            when {
            environment name: 'DEPLOY_TO', value:  'productions'
            }
            steps {
               echo "deploying"
            }
        }
    }
}
