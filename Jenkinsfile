pipeline {

  agent {
    node {
      label 'workstation'
    }
  }

  options {
    ansiColor('xterm')
  }

  environment {
    SAMPLE_URL="example.com"
  }

  stages {

    stage('one') {
      steps {
        sh 'echo hello world'
        sh 'echo ${SAMPLE_URL}'

      }
    }
  }
  post {
    always {
      sh 'echo post clean up steps'
    }
  }
}