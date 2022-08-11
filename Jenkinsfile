def x=10

pipeline  {
  agent any
   environment {
             x = 20 
             y = 30
  }
    parameters   {
      string(name: 'x', defaultValue: '30', description: 'Enter the value of x')
  }
  
  stages   {
     stage("1")      
    {
       
        steps       
        {
          echo "Stage1 -- Value of x is ${x} , env x is ${env.x} and y is {y}"
        }     
     }
      
     stage('2')       
    {
        
        steps
        {
            
          echo "Stage2 -- Value of x is  ${params.x}"
          echo "Stage2 -- Value of x is  ${env.x}"
        }     
     }  
   }
}
