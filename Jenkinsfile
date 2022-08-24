pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            echo 'hey'
            sleep 23
          }
        }

        stage('stage2') {
          steps {
            timeout(time: 23)
          }
        }

      }
    }

  }
  environment {
    DEMO = '1'
  }
}