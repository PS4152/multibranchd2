pipeline {
    agent any
    parameters {
        string(name: 'PERSON', defaultValue: 'mr jenkins', description: 'who shouid i say i hello ')
        text(name: 'BIOGRAPHY', defaultValue: '', description: 'enter the information below')
        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'picksomething')
        password(name: 'PASSWORD', defaultValue: 'secter', description: 'enter a password')
    }
    stages {
        stage ('build') {
            steps {
                echo "building ${PERSON}"
                echo "bio ${BIOGRAPHY}"
                echo "toggle ${TOGGLE}"  
                echo "paa ${ASSWORD}"          }
        }
    }
}
