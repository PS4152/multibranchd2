
pipeline {
    agent any
    stages {
        stage ('build') {
            steps {
                timeout (time: 300, unit:'SECONDS') {
                  input message:'are you building the application', ok: 'yes', submitter: 'sumanth'
                }
                
                echo "builing the application"
            }
        }
    }
}
