pipeline
{
	agent 
	{
		label 'built-in'
	}
	stages
	{
		/*stage ('install httpd')
		
			{
				steps
				{
					sh "yum install httpd -y"
				}
				
			}
		
		stage ('httpd start')
		
			{
				steps
				{
					sh "service httpd start"
				}
				
			}*/
		
		stage ('deploy index')
		
			{
				steps
				{
					sh "cp -r index.html /var/www/html"
					sh "chmod -R 777 /var/www/html/index.html"
					sh "service httpd restart"
				}
				
			}
		
			
	}
	
}
