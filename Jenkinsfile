def x = 10

pipeline  {
  agent any
  def y = 20
  
  stages   {
     stage("1")      
    {
       
        steps       
        {
             echo "Stage1 -- Value of x is  ${x}"
        }     
     }
      
     stage('2')       
    {
        steps
        {
             echo "Stage2 -- Value of y is  ${y}"
        }     
     }  
   }
}
