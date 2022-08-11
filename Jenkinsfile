pipeline 
{
  agent any
  environment
  {
      x = 10
  }
  stages
  {
     stage("1")
     {
        steps
        {
          echo "hello stage1 ${x}"
          echo "hello stage1 $x"
        }
     
     }
      
     stage('2')
     {
        steps
        {
             sh "echo stage2 ${x}"
             sh "echo stage2 $x"
             sh 'echo stage2 ${x}'
             sh 'echo stage2 $x'
        }
     
     }
  
  
   }

}
