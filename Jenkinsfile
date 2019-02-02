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
    stage('12') {
      parallel {
        stage('12') {
          steps {
            echo '12'
            sleep 5
          }
        }
        stage('21') {
          steps {
            echo '21'
            sleep 3
          }
        }
      }
    }
    stage('333') {
      steps {
        sh 'ls -l'
        sleep 10
      }
    }
  }
}