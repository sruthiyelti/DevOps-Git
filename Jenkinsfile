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
        Stage ('Nginxdeployment'){
           steps {
              node ('Build-nglnx') {
                 sh 'cp /home/ubuntu/workspace/nginxhtml/* /var/www/html/'
         
              }
           }
        }
     }
   
   
}
