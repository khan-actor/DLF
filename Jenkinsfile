pipeline {
	agent any 
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/owais/Documents/devopsoftware/apache-maven-3.9.5/bin/mvn install'
	                 }}
		stage('Deployment'){
		   steps {
		sh 'cp target/DLF.war /home/owais/Documents/devopsoftware/apache-tomcat-9.0.82/webapps'
			}}	
}}
