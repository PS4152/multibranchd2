pipeline {
    agent any
    stages {
        stage ("build") {
            steps {
                echo "buliding block"
            }
        }
        stage ("scrpiting") {
            steps {
                script {
                    def course = "docker"
                    if (course == "k8s") {
                        println("thanks for enrolling ${course}")
                    }
                    else
                    println("do enroll")
                }
            }
        }
    }
}
