ipeline {
   agent {
     label 'Build-nginx'
     }
     stages {
       stage ('Checkout') {
           steps {
             node ('Build-nginx') {
               checkout scm
             }
            }
        }      
     }
}
