inode ('built-in') {

    stage ('continuos download')
    {
        git branch: 'main', url: 'https://github.com/Veera6060/Scripted-Pipeline.git'
   }
    stage('continuos build')
    {
        sh 'mvn package'
    }
    stage('continuos delivery')
    {
        deploy adapters: [tomcat9(alternativeDeploymentContext: '', credentialsId: 'QASERVER', path: '', url: 'http://172.31.0.104:8080')], contextPath: 'testapp', war: '**/*.war'
    }
   }
