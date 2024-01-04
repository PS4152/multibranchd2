pipeline {
    agent any 
    stages {
        stage ("build") {
            steps {
                timeout(time: 180, unit: 'SECONDS') {
                    input(message: 'are u building block', ok: 'yes', submitter: 'sumanth')
                }
                echo "builing"
            }
        }
    }
}
