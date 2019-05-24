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
	sh 'cp -R $WORKSPACE/* /var/www/html/'	
	}
stage('restart_apache')
	{
	sh 'systemctl restart httpd'	
	}
	
}
