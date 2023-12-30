pipeline {
    agent any
    environment {
        name = "sumanth"
        course = "docker"
    }
    stages {
        stage ("build") {
            environment {
                cloud = "azure"
                name = "maha"
            }
            steps {
                echo "welcome to ${name} "
                echo "you are enrolled to ${course}"
                echo "you are enrolled to ${cloud}"
            }
        }
    }
}
