def server_id=Server
pipeline {
          agent {
		 label 'master'
	        }
	        stages {
		         stage ('checkout') {
			                     steps {
				                    node ('master') {
					                             checkout scm
				                                    }
			                            }
		                             }
                        }
           }
