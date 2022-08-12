def x = 10
def cmd1 = 'docker pull alpine:latest'
def cmd2 = 'docker images'
  
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
            sh "ssh -o StrictHostKeyChecking=no jenkins@52.87.228.97 ${cmd1}"
            sh "ssh -o StrictHostKeyChecking=no jenkins@52.87.228.97 ${cmd2}"
          }
        }     
     }  
   }
}
