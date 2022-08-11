def x=10

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
            
          echo "Stage2 -- Value of z is  ${x}"
        }     
     }  
   }
}
