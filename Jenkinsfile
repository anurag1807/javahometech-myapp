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
        def y = 20
        steps
        {
             echo "Stage2 -- Value of y is  ${y}"
        }     
     }  
   }
}
