pipeline {
    agent { node { label 'test_node' } }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            when {
                branch 'master'
            }
            steps {
                sh 'ls'
            }
        }
    }
}
