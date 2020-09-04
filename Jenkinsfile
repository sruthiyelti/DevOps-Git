pipeline {
   agent {
      label 'node-machine'
      }
   
     stages {
       stage ('Checkout') { 
           steps {
             node ('node-machine') {
               checkout scm
             }
            }
       
       }      
          
     }
}
