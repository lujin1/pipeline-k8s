pipeline {
  agent {
    kubernetes {
      label 'jenkins-node'
      containerTemplate {
        name 'jenkins-node'
        image 'wpacr.azurecr.io/jenkins-alpinenode:v3'
        ttyEnabled true
      }

    }

  }
  stages {
    stage('111') {
      parallel {
        stage('111') {
          steps {
            echo '123'
            sleep 40
          }
        }
        stage('222') {
          steps {
            echo '222'
            sleep 30
          }
        }
      }
    }
  }
}