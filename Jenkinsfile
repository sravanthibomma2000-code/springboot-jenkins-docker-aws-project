pipeline {
agent any

```
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
            echo 'Docker Build stage skipped temporarily'
        }
    }

    stage('DockerHub Push') {
        steps {
            echo 'DockerHub Push stage skipped temporarily'
        }
    }
}
```

}
