ipeline {
    agent any 
        parameters {
            string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
            text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')
            booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
            choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
        }
        stages {
            stage ('build') {
                steps {
                    echo "parametres ${PERSON}"
                    echo "hello ${BIOGRAPHY}"
                    echo "toggle ${TOGGLE}"
                    echo "choice ${CHOICE}"

                }
            }
        }
    }

