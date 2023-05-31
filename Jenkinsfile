pipeline {
    agent any
	tools {  
	  dockerTool 'mydocker'
	}
	stages {
	  stage('Example') {
	    steps {
		  sh 'docker --version'
		}
      stage('Build')
        steps {
            sh 'docker build -t pyhtonapp:v1 .'
        }
	}
}
}