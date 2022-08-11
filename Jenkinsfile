pipeline  {
  agent any
  parameters   {
      string(name: 'x', defaultValue: '10', description: 'Enter the value of x')
  }
  stages   {
     stage("1")      
    {
      environment {
             x = 20 
      }
        
        steps       
        {
             echo "Stage1 -- Value of x is  ${env.x}"
        }     
     }
      
     stage('2')       
    {
        steps
        {
             echo "Stage2 -- Value of x is  ${params.x}"
        }     
     }  
   }
}
