pipeline{
   agent any 
      stages{
	       stage("stage1"){
                           steps { 
						                         sh "yum install httpd -y" 						   
                                     sh "systemctl start httpd" 
                                     sh "cd /var/www/html"
                                     echo "this is my pipelinejob" >>/index.html 
                                     chmod 777 index.html									
									}
								}
								
								}
    
}
