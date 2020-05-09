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
                   bat "docker run hello-world" 
                   bat "kubectl get nodes"   
               }
           }
       }
   }
}
