pipeline {
    agent any
    //this env variables can be used across all the stages
    environment {
        //key value pairs
        name = "sumanth"
        course ="k8s"
    }
    stages {
        stage ("build") {
            //these environment varibles are specific to this stage only 19.25
            environment {
                 cloud = "GCP"

            }
            steps {
                echo "welcome ${name}"
                echo "you enrolled to ${course} course"
                echo "you are certified in ${cloud}"
            }
        }
    }
}
