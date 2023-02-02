pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo '"testing"'
          }
        }

        stage('Parallel') {
          steps {
            echo '"running environment"'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo '"building environment"'
      }
    }

    stage('Final') {
      steps {
        echo '"clean up"'
      }
    }

  }
}