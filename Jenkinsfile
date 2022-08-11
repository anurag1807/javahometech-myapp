def m = 99
  
pipeline  {
  agent any
   environment {
             x = 10
             z = 70
  }
    parameters   {
      string(name: 'x', defaultValue: '20', description: 'Enter the value of x')
  }
  
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

        environment {
             z = 99
        }      
        steps
        {
                  
          script {
                   def z = 50
                   env.z = 60
                   echo "Stage2 -- Script -- Value of z is  ${z} and env z is ${env.z}"
          }
          echo "Stage2 -- Value of x is  ${params.x}"
          echo "Stage2 -- Value of z is  ${z} and env z is ${env.z}"
        }     
     }  
   }
}
