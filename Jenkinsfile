pipeline{
    agent any

    stages{
        stage('build'){
            steps{
                echo'BRANCH_NAME : ${ env.BRANCHNAME_NAME}'
                echo'BRANCH_IS_PRIMARY : ${ env.BRANCHNAME_IS_PRIMARY}'
                echo'CI : ${ env.CI}'
                echo'BUILDER_NUMBER : ${ env.BUILDER_NUMBER}'
                echo'JENKINS_URL : ${ env.JENKINS_URL}'
            }
            
        }
    }
}