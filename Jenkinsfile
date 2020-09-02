pipeline {
   agent {
     label 'Build-nglnx'
     }
     stages {
       stage ('Checkout') {
           steps {
             node ('Build-nglnx') {
               checkout scm
             }
            }
       
       }      
        stage ('NginxDeployment'){
           steps {
              node ('Build-nglnx'){
                sh 'sudo cp /home/ubuntu/workspace/Project-gitPipeline/* /var/www/devops/ '
     
              
              }
           }
            
        }
              
              }
              
   
   
}
