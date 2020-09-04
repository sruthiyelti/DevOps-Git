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
          stage ('NginxDeployment'){
           steps {
              node ('node-machine'){
                sh 'sudo cp /home/ubuntu/workspace/git-integration/* /var/www/devops/ '
     
              
              }
           }
            
        }
     }
}
