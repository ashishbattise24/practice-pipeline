pipeline{
 agent {label 'node1'}
   
 parameters{
            choice(name: 'VERSION', choices: [1.2,1.3,104], description: "This is version value")
            booleanParam(name: 'execTest', defaultValue: true, description: "This is boolean value") 	
           } 
  stages{
         stage('Build'){
                         steps{
                                sh 'touch Buildpipe_new'
                                echo "Build Version ${NEW_VERSION}"
                                
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
