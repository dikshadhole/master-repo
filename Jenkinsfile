pipeline {
      agent {
             node { label "built-in"
				        customWorkspace "/mnt/22q2"
					 }
        }
		stages {
		
			stage ("22Q1"){
			
				steps {
		     
	            sh " rm -rf * "
                    sh ""
	            sh " docker run -itdp 81-85:80 --name testdev httpd "
	            sh " chmod -R 777 /mnt/22q2"
		    sh " docker cp /mnt/22q2/master-dev-qa-22q1-22q2-22q3/index.html testdev:/usr/local/apache2/htdocs "
                    
                    
				}
			}
		}
