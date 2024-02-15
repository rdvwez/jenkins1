pipeline{
    agent any
    // agent {
    //     docker{
    //         image 'node:21-alpine'
    //     }
    // }
    // option{
    //     timeout(time: 1, unit: "HOURS")
    // }

    // environment{
    //     MY_VAR = 'une variabale'
    //     MY_NUMBER = 123
    // }

    // stages{
    //     stage('build'){
    //         options{
    //             timestamps()
    //         }
    //         steps{
    //             sh 'npm -v'
    //         //     echo "BRANCH_NAME : ${ env.BRANCH_NAME }"
    //         //     echo "BRANCH_IS_PRIMARY : ${ env.BRANCH_IS_PRIMARY }"
    //         //     echo "CI : ${ env.CI }"
    //         //     echo "BUILD_NUMBER : ${ env.BUILD_NUMBer }"
    //         //     echo "JENKINS_URL : ${ env.JENKINS_URL }"
    //         //     echo "MY_VAR : ${ env.MY_VAR }"
    //         //     echo "MY_NUMBER : ${ env.MY_NUMBER }"

    //         //     sh 'printenv'
    //         }
            
    //     }
    // }

    // // post{
    // //     always{
    // //         echo 'always .... '
    // //     }
    // //     success{
    // //         echo 'success .... '
    // //     }
    // // }

    stages{

        // options{
        //     parallelAlwaysFailFast()
        // }

        stage('build'){
            failFast throw
            parallel{
                stage('build frontend'){
            steps{
                echo 'build frontend!'
            }
        }

        stage('build backend'){
            steps{
                echo 'build backend !'
            }
        }
            }
        }

        

        stage('deloyement production'){
            steps{
                echo 'deoy !'
            }
        }
    }

}