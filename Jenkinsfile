pipeline{
 agent {label 'node1'}
   
  stages{
         stage('init'){
                        steps{
                              script{
                                      gv = load "script.groovy"
                                    }  
                            }
                     }
         stage('Build'){
                         steps{
                               script{
                                      gv.buildApp()  
                               }
                                                                
                              }
                       }
         stage('Deploy'){
                       steps{
                             script{
                                    gv.deployApp()
                             }
                            }
                      }
       
 
       }

       }  
