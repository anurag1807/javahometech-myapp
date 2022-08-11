pipeline  {
  agent any
  environment   {
      x = 1
  }
  stages   {
     stage("1")      {
        environment         {
            x = 3
            y = 4
        }
        steps         {
            script {
            env.x = 5
            env.y = 6
          }
            echo "Stage1 -- Valkue of x is  ${x}"
            echo "Stage1 -- Valkue of y is  ${y}"
        }     
     }
      
     stage('2')       {
        steps
        {
             echo "Stage2 -- Valkue of x is  ${x}"
             echo "Stage2 -- Valkue of y is  ${y}"
        }     
     }  
   }
}
