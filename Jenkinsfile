node 
{
	stage('declareEnvVariables')
	{
        def WORKSPACE = "/var/lib/jenkins/workspace/phpProject_cicd"
        }
stage('gitCheckout') 
	{
        checkout scm
    	}
stage('Deploy')
	{
	sh 'cp -r $WORKSPACE/* /var/www/html/'	
	}
	
}
