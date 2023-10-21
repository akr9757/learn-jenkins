pipeline {

  agent {
    node {
      label 'workstation'
    }
  }

  stages {

    stage('one') {
      steps {
        sh 'echo hello world'
      }
    }
  }
  post {
    always {
      sh 'echo post clean up steps'
    }
  }
}