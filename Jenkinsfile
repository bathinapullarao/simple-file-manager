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
	sh 'rm -rvf /var/www/html/*'
	sh 'cp -R $WORKSPACE/* /var/www/html/'	
	}
}
