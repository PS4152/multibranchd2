pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('deploy') {
            when {
                not {
                 equals expected: 'production', actual: 'DEPLOY_TO'
                }
            }
            steps {
               echo "deploying"
            }
        }
    }
}
