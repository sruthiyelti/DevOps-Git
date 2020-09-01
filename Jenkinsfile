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
     }
}
