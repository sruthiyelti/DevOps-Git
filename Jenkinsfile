pipeline {
   agent {
     label 'Build-nglnx'
     }
    parameters 
    
           choice(choices: 'develop\nrelease\nmaster', description: 'select the branch name ' , name: 'Branch_Name')
     
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
