pipeline {
 agent {label 'node1'}

 stages{
       stage("Build"){
                       steps{
                               sh 'touch Build_file'
                            }
                     }
       stage("Prod"){
                       steps{
                               sh 'touch Prod_file'
                            }
                    }
  
       }
}
