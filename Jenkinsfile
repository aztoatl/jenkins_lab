def agent_label
if (BRANCH_NAME == "dev") {
    agentLabel = "dev_node"
} else {
    agentLabel = "test_node"
}

pipeline {
    agent { label agent_label }        
stage('build') {
            when {
                branch 'master'
            }
            
            steps {
              script{
                ls
              }
            }
        }
        when {
                branch 'dev'
            }
            steps {
                 script{
                ls
              }
            }
        
}
