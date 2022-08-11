pipeline  {
  agent any
  parameters   {
      string(name: 'x', defaultValue: '10', description: 'Enter the value of x')
  }
  stages   {
     stage("1")      
    {
       
        steps         
        {
            parameters   
            {
             string(name: 'x', defaultValue: '20', description: 'Enter the value of x')
            }
          echo "Stage1 -- Value of x is  ${params.x}"
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
