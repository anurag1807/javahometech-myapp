pipeline 
{
  agent any
  environment
  {
      x = 10
  }
  stages
  {
     stage("1")
     {
       
        steps
        {
          
          env.x = 20
          env.y = 30
          echo "hello stage1 ${x}"
          echo "hello stage1 ${env.y}"
        }
     
     }
      
     stage('2')
     {
        steps
        {
             sh "echo stage2 ${x}"
             echo "hello stage2 ${env.y}"
        }
     
     }
  
  
   }

}
