pipeline{
    agent none 
    stages{
            stage("build"){
                agent { label "build" }
                steps{
                    echo "building..."
                    script{
                        sh "sleep 10"
                    }
                }
            }
        
    }
     post{
         always{
            script{
                println("流水线结束后，经常做的事情")
            }
         }
         success{
            script{
                println("流水线成功后，经常做的事情")
            }
         }
         failure{
            script{
                println("流水线失败后，经常做的事情")
            }
         }
         aborted{
            script{
                println("流水线取消后，经常做的事情")
            }
         }
     }
}