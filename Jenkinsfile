pipeline {
    agent any
    stages {
        stage ('UAT') {
            when {
                branch 'release-*'
            }
            steps {
                echo "deploying to stage"
            }
        }
        stage ('prod') {
            when {
                tag pattern: "v\\d{1,2}.\\d{1,2}.\\d{1,2}",comparator: REGEXP
            }
            steps {
                echo "deploying to production environment"
            }
        }
    }
}
