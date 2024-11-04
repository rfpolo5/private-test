pipeline{
    agent {
        node { label "Develoment"
        }
    }

    stages{
        stege("build"){
            steps{


                echo "building in ${env.NODE_NAME} and executor ${env.EXECUTOR_NUMBER}"
            }
        }

        stage("test"){
            steps{
                echo "TESTING in ${env.NODE_NAME} and executor ${env.EXECUTOR_NUMBER}"
                
            }
        }

        stage("deploy"){
            steps{
                echo "DEPLOY in ${env.NODE_NAME} and executor ${env.EXECUTOR_NUMBER}"

            }
        }
    }

    post{

        always{
        
            echo "test always"
        }
        success{
            echo "bien "
        }
        failure{
            echo "fail"
        }
    }

}
