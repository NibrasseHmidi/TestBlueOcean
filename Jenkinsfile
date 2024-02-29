pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'build completed '
      }
    }

    stage('test stages ') {
      parallel {
        stage('test2') {
          steps {
            echo 'Running test2'
          }
        }

        stage('test1') {
          steps {
            echo 'Running test1'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployment completed'
      }
    }

  }
}