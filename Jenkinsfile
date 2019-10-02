stage('build') {
            when {
                branch 'master'
            }
            steps {
              script{
                echo 'Hi Master'
              }
            }
        }
        stage('build') {
            when {
                branch 'dev'
            }
            steps {
                 script{
                echo 'Hi Dev'
              }
            }
        }
