pipeline{
 agent {label 'node1'}
   
 parameters{
            string(name: 'VERSION', defaultValue: '', description: "This is string")
            choice(name: 'VERSION', choices[1.2,1.3,104], description: "This is version value")
            booleanParam(name: execTest, defaultValue: true, description: "This is boolean value") 	
 } 
  stages{
         stage('Build'){
                         steps{
                                sh 'touch Buildpipe_new'
                                echo "Build Version ${NEW_VERSION}"
                                withCredentials([
                                   usernamePassword(credential: 'ans-id', usernameVariable: USER, passwordVariable: PWD)]
                                 {
                                  sh "username ${USER} and passwd is ${PWD}"
                                }
                                
                              }
                       }
         stage('Prod'){
                       steps{
                              sh 'touch Prodpipe_new'
                              echo "Build Version is ${params.VERSION}"
                            }
                      }
       
 
       }

       }  
