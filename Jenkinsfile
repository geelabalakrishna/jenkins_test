pipeline {
    agent any
    stages {
        // Stage for an exact branch match using EQUALS
        stage('Parallel Stage') {       
            parallel {
                stage('Master Branch Build_main') {
                    when {
                        branch pattern: "main", comparator: "EQUALS"
                    }
                    steps {
                        echo 'Running on the master branch only'
                        // Add additional steps for master branch
                    }
                }
                stage('Master Branch Build_dev') {
                    when {
                        branch pattern: "dev", comparator: "EQUALS"
                    }
                    steps {
                        echo 'Running on the master branch only'
                        // Add additional steps for master branch
                    }
                } 
            }
        }           
    
    }

}  
