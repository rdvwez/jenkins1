pipeline{
    agent {
        docker{
            image 'node:21-alpine'
        }
    }

    environment{
        MY_VAR = 'une variabale'
        MY_NUMBER = 123
    }

    stages{
        stage('build'){
            steps{
                sh 'npm -v'
            //     echo "BRANCH_NAME : ${ env.BRANCH_NAME }"
            //     echo "BRANCH_IS_PRIMARY : ${ env.BRANCH_IS_PRIMARY }"
            //     echo "CI : ${ env.CI }"
            //     echo "BUILD_NUMBER : ${ env.BUILD_NUMBer }"
            //     echo "JENKINS_URL : ${ env.JENKINS_URL }"
            //     echo "MY_VAR : ${ env.MY_VAR }"
            //     echo "MY_NUMBER : ${ env.MY_NUMBER }"

            //     sh 'printenv'
            }
            
        }
    }

    // post{
    //     always{
    //         echo 'always .... '
    //     }
    //     success{
    //         echo 'success .... '
    //     }
    // }
}