
pipeline {
    agent any 
    stages {
        stage ('build') {
            steps {
                timeout(time: 180, unit: 'SECONDS') {
                    input message: 'are you building', ok: 'yes', submitter: 'sumanth'
                }
                echo "builing application sucess"
            }
        }
    }
}
