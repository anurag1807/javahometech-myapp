def x = 10
  
pipeline  {
  agent any  
  stages   {
     stage("1")      
    {   
        steps       
        {
          echo "Stage1 -- Value of x is ${x}"
        }     
     }
      
     stage('2')       
    {   
        steps
        {
          sshagent(['server2-cred']) {
            sh 'ssh -o StrictHostKeyChecking=no jenkins@52.87.228.97 docker pull alpine:latest'
            sh 'ssh -o StrictHostKeyChecking=no jenkins@52.87.228.97 docker images'
          }
        }     
     }  
   }
}
