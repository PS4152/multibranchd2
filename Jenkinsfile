pipeline {
    agent any 
    stages {
        stage ('build') {
            timeout (time: 180, unit:'SECONDS')  {
                input (message: 'are you building', ok: 'yes', submitter: 'sumanth')
            }
            echo "are building sucess"
        }
    }
}
