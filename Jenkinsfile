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
        stage('Build') {
            when {branch 'master'}
            steps {sh 'ls'}
            when{branch 'dev'}
            steps {sh 'ls'}
        }
    }
}
