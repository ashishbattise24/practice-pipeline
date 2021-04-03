pipeline{
 agent {label 'node1'}
 environment {
               NEW_VERSION = '3.1.0'
               SERVER_CREDENTIAL = credentials('ans-id')
 } 
  stages{
         stage('Build'){
                         steps{
                                sh 'touch Buildpipe_new'
                                echo "Build Version ${NEW_VERSION}"
                                echo "credentails are ${SERVER_CREDENTIAL}"
                              }
                       }
         stage('Prod'){
                       steps{
                              sh 'touch Prodpipe_new'
                            }
                      }
       
 
       }

       }  
