pipeline {
    agent any
    stages {
        stage ('build') {
            steps {
                echo "executing multi branch pipeline"
            }
        }
        stage ('test') {
            steps {
                echo "excuting test stage"
            }
        }
        stage ('deploytodev') {
            steps {
                echo "excuting dev deployment stage"
            }
        }
        stage ('deploytoprods') {
            steps {
                echo "executing prod deployment stage"
            }
        }
    }
}
