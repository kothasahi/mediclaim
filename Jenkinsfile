pipeline {
	   agent any
		environment {
	       PATH = "/opt/maven/bin:$PATH"
	}
		stages {
	      stage('Git Checkout') {
	         steps {
	            git 'https://github.com/saidevmalik/mediclaim.git'
			}
		}
		stage('Build') {
		steps {
		sh '/opt/maven/bin/mvn clean install'
			}
		}
	}
		}
}
