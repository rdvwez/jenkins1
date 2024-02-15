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



    // ---------------------------------- Notions de stages parralle
    // stages{

    //     // options{
    //     //     parallelAlwaysFailFast()
    //     // }

    //     stage('build'){
    //         failFast true
    //         parallel{
    //             stage('build frontend'){
    //         steps{
    //             echo 'build frontend!'
    //         }
    //     }

    //     stage('build backend'){
    //         steps{
    //             echo 'build backend !'
    //         }
    //     }
    //         }
    //     }
    //     stage('deloyement production'){
    //         steps{
    //             echo 'deploy !'
    //         }
    //     }
    // }



    // ---------------------------------- Notions de matrice
    // stages{
    //     stage('build and test'){
    //         matrix{
    //             axes{
    //                 axis{
    //                     name 'PLATEFORM'
    //                     values 'linux', 'macos', 'windows'
    //                 }
    //                 axis{
    //                     name 'BROWSER'
    //                     values 'firefox', 'chrome', 'safari'
    //                 }
    //             }
    //             stages{
    //                 stage('build'){
    //                     steps{
    //                         echo "construire pour ${ PLATEFORM } - ${BROWSER}"
    //                     }
    //                 }
    //                 stage('test'){
    //                     steps{
    //                         echo "test pour ${ PLATEFORM } - ${BROWSER}"
    //                     }
    //                 }
    //             }
    //         }
    //     }
    //     stage('deployement production'){
    //         steps{
    //             echo "====++++deloy !++++===="
    //         }
    //     }
    // }

    // ---------------------------------------Notions d'artefacte

    stages[
        stage('build'){
            steps{
                sh 'echo hello > world.txt'
                archiveArtefacts(artifacts: '*.txt')
            }
        }
    ]

}