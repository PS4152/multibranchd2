pipeline {
    agent any 
    stages {
        stage ('build') {
            when {
                branch 'release/*'
            }
            steps {
                echo "weclome to pipeline"
            }
        }
    }
}
