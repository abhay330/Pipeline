#!groovy

pipeline {
	environment {
		GIT_PROJECT_URL = "https://github.com/abhay330/Pipeline.git"
	}

	agent {
		node {
			label "Windows"
			customWorkspace "workspace/${JOB_NAME}"
		}
	}
	
	stages {
		stage ("Prepare") {
			steps {
				script {
					cleanWS()
				}
			}
		}
		stage ("Checkout") {
			steps {
				script {
					checkout scm
				}
			}
		}		
	}
}