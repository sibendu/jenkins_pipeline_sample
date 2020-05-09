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
                   echo "Build stage"         
                   bat "docker run hello-world" 
                   bat "kubectl get nodes"   
               }
           }
       }
       stage('Deploy') {
           steps {
               script{
                   echo "Deploy stage"         
                   bat "kubectl get pods"   
               }
           }
       }
   }
}
