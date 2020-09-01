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
        stage ('Nginxdeployment'){
           steps {
              node ('Build-nglnx') {
                 sh 'sudo cp /home/ubuntu/workspace/nginxhtml/* /var/www/html/'
         
              }
           }
        }
     }
   
   
}
