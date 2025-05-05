pipeline {

	agent {

			label {

					label "built-in"
					customWorkspace "/mnt/test"	
			}
		}


		stages {


			stage ('one') {

					steps {

						echo "hello velocity"
					}
			}

			stage ('two') {

					steps {
						sh "yum install httpd -y"
						sh "cp index.html /var/www/html/"
						sh "service httpd start"
						sh "chmod -R 777 /var/www/html/index.html"
						
					}
			}

		}

}
