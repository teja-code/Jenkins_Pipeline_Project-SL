pipeline {
    agent any

    stages {
        stage('Checkout source code') {
            steps {
                echo "Getting source code"
                git 'https://github.com/teja-code/Projectdemo.git'
            }
        }
/*        stage('Checkout') {
            steps {
                script {
                    def commitId = env.CHANGE_ID
                    echo "GitHub Commit ID: ${commitId}"
                }
            }
        }
        stage('Build Docker image') {
            steps {
                echo "Build Docker image"
                sh "docker image build -t img_${commitId} ."
            }
        }
        stage('create container') {
            steps {
                echo "create container"
                sh "docker container run -p 8083:80 --name cont_${commitId} img_${commitId}"
                sh "docker container ls"
            }
        }
        stage('Push docker image to Dockerhub') {
            steps {
                echo "Push docker image to Dockerhub"
                // Log in to Docker Hub
                sh "docker login -u SaiTejaChandragiri -p Fubuki@123"
                
                sh "docker push demoimg"
            }
        }
        stage('Pull image and create container') {
            steps {
                echo "Pull image and create container"
                sh "docker pull demoimg"
                sh "sudo docker container run -p 8080:80 --name democont demoimg"
            }
        }*/
    }
}
