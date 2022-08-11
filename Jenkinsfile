def x=1000

pipeline  {
  agent any
   environment {
             x = 20 
  }
    parameters   {
      string(name: 'x', defaultValue: '30', description: 'Enter the value of x')
  }
  
  stages   {
     stage("1")      
    {
       
        steps       
        {
             echo "Stage1 -- Value of x ${x}"
        }     
     }
      
     stage('2')       
    {
        
        steps
        {
            
          echo "Stage2 -- Value of x is  ${params.x}"
          echo "Stage2 -- Value of x is  ${x}"
        }     
     }  
   }
}
