pipeline {
    agent any
    parameters {
        // string, text, boolen, choice, password 
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
        string(name: 'BRANCH_NAME', defaultValue: 'main', description: 'whats the branch i should build?')
    }
    stages {
        stage ('example') {
            steps {
              echo "hello siva"
            }
        }
    }

}
