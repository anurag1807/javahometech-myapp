pipeline 
{
  agent any
  
  stages
  {
     stage("1")
     {
        steps
        {
             echo "hello stage1"
        }
     
     }
      
     stage('2')
     {
        steps
        {
             echo "hello stage2"
             sh "echo inside double quotes"
             sh 'echo inside single quotes'
             sh echo "hellow world"
        }
     
     }
  
  
   }

}
