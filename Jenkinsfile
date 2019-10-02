def agentLabel
if (BRANCH_NAME == 'master') {
    agentLabel = 'test_node'
} else {
    agentLabel = 'dev_node'
}


pipeline {
    agent { node { label agentLabel } }
    environment {
        CI = 'true'
    }
    stages {
        stage('Test') {
            when {branch 'master'}
            steps {sh 'ls'}
        }
        stage('Dev') {
            when {branch 'dev'}
            steps {sh 'ls'}
        }
    }
}
