pipeline {
   agent {
     label 'node'
     }
    parameters 
    
           choice(choices: 'develop\nrelease\nmaster', description: 'select the branch name ' , name: 'Branch_Name')
     
    }
     stages {
       stage ('Checkout') {
           steps {
             node ('node') {
               checkout scm
             }
            }
       
       }      
       
              
              }
              
   
   
}
