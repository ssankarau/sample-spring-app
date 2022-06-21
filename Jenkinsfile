pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                echo "Build the Docker Image"
            }
        }
        stage("upload Artifacts") {
            steps {
                echo "Upload Docker Image to Docker Hub"
            }
        }
        stage("Deploy Docker Image") {
            steps {
                echo "Deploy Spring boot Application"
            }
        }
    }
}