pipeline {
    agent any
    
    stages {
        stage('Example Stage') {
          when { expression { env.BRANCH_NAME=='master'}
               }
            steps {
                echo 'This is an example echo statement in MASTER'
            }

           stage('Example Stage')
            when { expression { env.BRANCH_NAME=='main'}
               }{
            steps {
                echo 'This is an example echo statement in main'
            }

              stage('Example Stage')
                when { expression { env.BRANCH_NAME=~'main'}
               }{
            steps {
                echo 'This is an example echo statement in doestnt container main'
            }
        }
    }
}
