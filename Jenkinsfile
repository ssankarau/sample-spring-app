pipeline {
    agent any
    stages {
        stage("Build") {
            agent {
                docker-agent {
                    image 'jenkins/agent'
                }
            }      
            steps {
                echo "Build the Docker Image"
                sh "docker build . -t ssankarmca37/my-spring-app:${BUILD_NUMBER}"
            }
        }
        stage("Upload Artifacts") {
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