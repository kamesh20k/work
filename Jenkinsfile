pipeline {
    agent any
    
    stages {
        stage('Example Stage - Master Branch') {
            when {
                expression { env.BRANCH_NAME == 'master' }
            }
            steps {
                echo 'This is an example echo statement in the master branch'
            }
        }
        
        stage('Example Stage - Main Branch') {
            when {
                expression { env.BRANCH_NAME == 'main' }
            }
            steps {
                echo 'This is an example echo statement in the main branch'
            }
        }
        
        stage('Example Stage - Main Container Branch') {
            when {
                expression { env.BRANCH_NAME != 'main' }
            }
            steps {
                echo 'This is an example echo statement in a main container branch'
            }
        }
    }
}
