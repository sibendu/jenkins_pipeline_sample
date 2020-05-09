pipeline {
   agent any
   environment {
       registry = "sibendudas/k8scicd"    
       GOCACHE = "/tmp"
   }
   stages {
       stage('Build') {
           steps {
               script{
                   echo "Hello World!"    
                   bat "docker ps" 
                   bat "kubectl get nodes"   
               }
           }
       }
   }
}
