#!groovy

pipeline {
	environment {
		GIT_PROJECT_URL = "https://github.com/abhay330/Pipeline.git"
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

	post {
	}
}