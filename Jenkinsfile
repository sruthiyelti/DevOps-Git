pipeline {
   agent {
      label 'node-machine'
      }
    parameters 
    
           choice(choices: 'develop\nrelease\nmaster', description: 'select the branch name ' , name: 'Branch_Name')
     
    }
     stages {
       stage ('Checkout') { 
           steps {
             node ('node-machine') {
               checkout scm
             }
            }
       
       }      
          stage ('clean package') {
            steps {
               node ('node-machine') {
                 sh 'mvn package'
               }
              }
              
              }
              
   
   
}
