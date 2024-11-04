pipeline{
    agent any
    stages{
        stage('stage_1'){
            when{
                allOf{
                    branch 'main'      // Condition 1: Current branch is master
                    branch 'dev'     // Condition 2: Current branch is develop
                    branch  'prod'
                }
            }
            steps{
                echo 'stage1_step1'
            }
        }
    }
} 
