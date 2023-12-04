pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'this is dev'
      }
    }

    stage('build') {
      steps {
        echo 'this is build'
      }
    }

    stage('test') {
      steps {
        echo 'this is step'
      }
    }

    stage('UAT') {
      parallel {
        stage('UAT') {
          steps {
            echo 'this is UAT'
          }
        }

        stage('deploy') {
          steps {
            echo 'this is deploy'
          }
        }

        stage('operate') {
          steps {
            echo 'this is operate'
          }
        }

      }
    }

  }
}