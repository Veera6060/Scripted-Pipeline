node ('built-in') {

    stage ('continuos download')
    {
        git branch: 'main', url: 'https://github.com/Veera6060/Scripted-Pipeline.git'
   }
    stage('continuos build')
    {
        sh 'mvn package'
    }
   
   }
