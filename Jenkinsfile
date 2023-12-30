pipeline {
    agent any
    environment {
        name = "sumanth"
        course = "k8s"
    }
    stages {
        stage ("build") {
            environment {
                cloud = "gcp"
            }
            steps {
                echo "welcome ${name}"
                echo "you enrolled to ${course} course"
                echo "you are certified in ${cloud}"
            }
        }
        stage ('secondstage') {
            environment {
                cloud = "AWS"
            }
           steps {
            echo "welcome ${name}"
            echo "you enrolled to ${course} course"
            echo "you are certified in ${cloud}"
           }
        }
    }
}
