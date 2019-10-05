#!groovy

pipeline {
	environment {
		GIT_PROJECT_URL = "https://github.com/abhay330/Pipeline.git"
		VERSION = "1.01"
	}

	agent {
		node {
			label ""
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
