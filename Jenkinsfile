node('built-in') 
{
    stage('Continuous Download') 
    {
      git branch: 'main', url: 'https://github.com/Veera6060/Scripted-Pipeline.git'

     try
     {
        sh 'mvn package'  //This might Fail

     }

     catch (Exception e)
     {
      echo "Build is Faild"
      // Email Notification

      mail bcc: '', body: 'CI CD & CD Faild', cc: 'vvkr6060@gmail.com', from: '', replyTo: '', subject: 'CI_CD_Process', to: 'vvkr6060@gmail.com'
      exit(1)
     }
    }
}
