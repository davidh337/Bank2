pipeline {
  agent any
  stages {
    stage('Buid') {
      steps {
        sh 'echo 1'
        sh 'echo 2'
      }
    }

    stage('Test') {
      steps {
        sh 'echo 3'
      }
    }

    stage('Step 3') {
      parallel {
        stage('Step 3') {
          steps {
            sh 'echo step3'
          }
        }

        stage('step31') {
          steps {
            sh 'echo step31'
          }
        }

      }
    }

  }
}