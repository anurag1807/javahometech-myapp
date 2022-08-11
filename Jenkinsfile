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
                   def x = 50
                   echo "Stage2 -- Script -- Value of x is  ${x}"
          }
          echo "Stage2 -- Value of x is  ${x}"
        }     
     }  
   }
}
