pipeline {
  agent any
  stages {
  stage('Stage 1') {
      when {
          branch 'master'
          steps {
            script {
              echo 'Master'
            }
          }
      }
      when {
          branch 'dev'
          steps {
            script {
              echo 'dev'
            }
          }
      }

    }

  }
}
