pipeline {
      agent {
             node { label "built-in"
				        customWorkspace "/mnt/22q1"
					 }
        }
		stages {
		
			stage ("22Q1"){
			
				steps {
		
                    sh " rm -rf * "
		                sh "https://github.com/dikshadhole/master-repo.git"
	                        sh " docker run -itdp 81-85:80 --name testmaster httpd "
	                        sh " chmod -R 777 /mnt/22q1 "
		                sh " docker cp /mnt/22q1/master-dev-qa-22q1-22q2-22q3/index.html testmaster:/usr/local/apache2/htdocs "
                    
                    
				}
			}
		}
}
