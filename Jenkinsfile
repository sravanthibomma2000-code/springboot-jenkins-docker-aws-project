pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git branch: 'main',
                url: 'https://github.com/sravanthibomma2000-code/springboot-jenkins-docker-aws-project.git'
            }
        }

        stage('Build') {
            steps {
                sh 'chmod +x mvnw'
                sh './mvnw clean package -DskipTests'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t petclinic:v3 .'
            }
        }

        stage('DockerHub Push') {
            steps {
                withCredentials([usernamePassword(
                    credentialsId: 'dockerhub-creds',
                    usernameVariable: 'DOCKER_USER',
                    passwordVariable: 'DOCKER_PASS'
                )]) {

                    sh '''
                    docker login -u $DOCKER_USER -p $DOCKER_PASS
                    docker tag petclinic:v3 sravanthibomma2000/petclinic:v3
                    docker push sravanthibomma2000/petclinic:v3
                    '''
                }
            }
        }
    }
}
