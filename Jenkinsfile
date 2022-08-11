pipeline 
{
  agent any
  environment
  {
      x = 1
      y = 2
  }
  stages
  {
     stage("1")
     {
       
        steps
        {
          script {
          env.x = 5
          env.y = 6
          }
          echo "hello stage1 ${x}"
          echo "hello stage1 ${y}"
        }
     
     }
      
     stage('2')
     {
        steps
        {
             sh "echo stage2 ${x}"
             echo "hello stage2 ${y}"
        }
     
     }
  
  
   }

}
