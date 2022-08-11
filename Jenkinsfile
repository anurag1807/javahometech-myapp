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
                  
          script {
                   def z = 50
                   echo "Stage2 -- Script -- Value of z is  ${z}"
          }
          echo "Stage2 -- Value of x is  ${x}"
        }     
     }  
   }
}
