pipeline  {
  agent any
  parameters   {
      string(name: "x", defaultValue: "10", Description: "Enter the value")
  }
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
             echo "Stage2 -- Value of x is  ${x}"
        }     
     }  
   }
}
