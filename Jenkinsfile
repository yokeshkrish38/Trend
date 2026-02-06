pipeline {
  agent any

  stages {

    stage('Clone Repo') {
      steps {
        git 'https://github.com/yokeshkrish38/Trend.git'
      }
    }

    stage('Build Docker Image') {
      steps {
        sh 'docker build -t krish96/trend-app:latest .'
      }
    }

    stage('Push Image to DockerHub') {
      steps {
        withCredentials([usernamePassword(
          credentialsId: 'dockerhub-creds',
          usernameVariable: 'USER',
          passwordVariable: 'PASS'
        )]) {
          sh '''
            echo $PASS | docker login -u $USER --password-stdin
            docker push krish96/trend-app:latest
          '''
        }
      }
    }

    stage('Deploy to Kubernetes') {
      steps {
        sh '''
          kubectl apply -f deployment.yaml
          kubectl apply -f service.yaml
        '''
      }
    }
  }
}

