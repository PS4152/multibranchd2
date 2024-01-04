pipeline {
    agent any
    parameters {
        // string, text, boolen, choice, password 
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
        string(name: 'BRANCH_NAME', defaultValue: 'main', description: 'whats the branch i should build?')
        boolenParam(
            name: 'TOOGLE',
            defaultValue: true
            description: 'toogle this value'
        )
        choice(
            name: 'ENV',
            choices: ['dev', 'tst', 'stg', 'prd'],
            description :'select the env u want to deploy'
        )
    }
    stages {
        stage ('example') {
            steps {
              echo "hello ${params.PERSON}"
              echo "boolen parameter is: ${params.TOOGLE}"
              ECHO "Deploying to ${params.ENV} environment"
            }
        }
    }

}
