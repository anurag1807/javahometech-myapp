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
          sh 'mvn package'
        }     
     }  
   }
}
