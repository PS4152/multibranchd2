pipeline {
    agent any
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('deploy') {
            when {
            
            //equals expected: 5,actual: "${BUILD_NUMBER}"
             equals expected: 5, actual: currentBuild.number 
            }
            steps {
               echo "deploying"
            }
        }
    }
}
