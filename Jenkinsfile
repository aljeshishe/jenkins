pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'param=$(param)'
            sh 'touch 1'
          }
        }
        stage('alternative') {
          steps {
            echo 'alternative'
          }
        }
      }
    }
    stage('Test') {
      steps {
        echo 'Test'
        sh 'touch 2'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy'
        sh 'touch 3'
      }
    }
  }
}
