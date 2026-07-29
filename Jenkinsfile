node('built-in') 
{
    stage('Continuous Download') 
    {
      git branch: 'main', url: 'https://github.com/Veera6060/Scripted-Pipeline.git'
    }
 
     stage ('continuos buld'){
        sh 'mvn package'  //This might Fail

     }

    
    }
}
