pipeline {
  agent {
    kubernetes {
      //cloud 'kubernetes'
      label 'jenkins-node'
      containerTemplate {
        name 'jenkins-node'
        image 'wpacr.azurecr.io/jenkins-alpinenode:v3'
        ttyEnabled true
        // command 'cat'
      }
    }
  }
  stages {
    stage('111') {
      steps {
        echo '123'
      }
    }
  }
}
