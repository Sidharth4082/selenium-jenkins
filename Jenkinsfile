pipeline {
    agent any
	tools {  
	  dockerTool 'mydocker'
	}
    stages {
        stage('Hello') {
            steps {
                sh 'docker --version'
            }
        }
		stage("Build") {
			steps {
				sh 'docker build -t python:v1 .'
			}
		}
    }
}