pipeline{
    //agent any
    //agent { label "build" }
    agent {
        node {
            label "build"
            customWorkspace "/opt/agent/workspace"
        }
    }
    stages {
        stage("hello"){
            steps{
                echo "agent/node"
            }
        }
    }

}