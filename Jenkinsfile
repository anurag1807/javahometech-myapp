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
       
        environment
        {
           x = 3
           y = 4
        }
        steps
        {
          script {
          env.x = 5
          env.y = 6
          }
          echo "hello  ${x}"
          echo "hello  ${y}"
        }
     
     }
      
     stage('2')
     {
        steps
        {
             echo "hello  ${x}"
             echo "hello  ${y}"
        }
     
     }
  
  
   }

}
