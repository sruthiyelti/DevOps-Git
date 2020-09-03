pipeline {
   agent any
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
          stage ('clean package') {
            steps {
               node ('node') {
                 sh 'mvn package'
               }
              }
              
              }
              
   
   
}
