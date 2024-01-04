pipeline {
    agent any 
    stages {
        stage ('build') {
            steps {
                timeout (time: 180, unit:'SECONDS') {
                    input(message: 'are you', ok: 'yes', submitter: 'sumanth')
                }
            }
        }
    }
}
