def x = 10

pipeline  {
  agent any
  stages   {
     stage("1")      
    {
       
        steps       
        {
             echo "Stage1 -- Value of x   ${x}"
        }     
     }
      
     stage('2')       
    {
        
        steps
        {
            script {  
                   def y = 20 
                   echo "Stage2 -- Value of y is  ${y}"
                   env.z = y
             }
          echo "Stage2 -- Value of z is  ${z}"
        }     
     }  
   }
}
