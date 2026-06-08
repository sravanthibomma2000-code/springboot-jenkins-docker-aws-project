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
