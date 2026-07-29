node('built-in') 
{
    stage('Continuous Download') 
    {
      git branch: 'main', url: 'https://github.com/Veera6060/Scripted-Pipeline.git'
    }
     stage('Continuous Build') 
    {
     sh 'mvn package'
    }

}
