pipeline {
	agent any
	tools {
    	maven 'Maven_Home'
      jdk 'AmazonLinuxEC2'
	}
	stages {
    	stage("Checkout") {   
        	steps {               	 
            	git url: 'https://github.com/nagenn/testpipe'          	 
           	 
        	}    
    	}
    	stage('Build') {
        	steps {
        	sh "mvn compile"  	 
        	}
    	}
   	 
    	stage("Unit test") {          	 
        	steps {  	 
            	sh "mvn test"          	 
       	}
    }
  }
}
