properties([pipelineTriggers([githubPush()])])
 
pipeline {
    agent {
        label 'master'
    }
 
    stages {
         stage('Do the deployment') {
            steps {
                echo ">> Run deploy applications "
            }
        }
    }
 
    /* Cleanup workspace */
    post {
       always {
           deleteDir()
       }
   }
}
