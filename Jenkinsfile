pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh '''
              echo \'Build\'
            '''
          }
        }

        stage('Build2') {
          steps {
            sh 'echo \'Build2\''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        sh '''sleep 1
echo \'Deploy\''''
      }
    }

  }
}