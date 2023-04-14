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
            echo '"testing" '
          }
        }

        stage('parallel step') {
          steps {
            echo 'parallel step'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'building'
      }
    }

    stage('Clean up') {
      steps {
        echo 'cleaning'
      }
    }

  }
}