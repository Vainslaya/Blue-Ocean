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
            echo 'Testing'
          }
        }

        stage('Parallel') {
          steps {
            echo 'Parallel'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'Build'
      }
    }

    stage('Clean up') {
      steps {
        echo 'Cleaning'
      }
    }

  }
}