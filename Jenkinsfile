
pipeline {
    agent any 
    stages {
        stage ('buid') {
            steps {
                timeout (time: 180, unit: 'SECONDS')
                input message: 'are you build', ok: 'yes', submitter: 'sumanth'
            }
            echo "building the application"
        }
    }
}
