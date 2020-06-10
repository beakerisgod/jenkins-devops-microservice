//SCRIPTED

//DECLARATIVE
pipeline {
	agent any
	//agent { docker { image 'maven:3.6.3'} }
	//agent { docker {image 'node:13.8'} }
	stages {
		stage('Build') {
			steps {
				// echo 'node --version'
				echo "Build"
				echo "$PATH" - $PATH"
				echo "BUILD_NUMBER" - $env.BUILD_NUMBER"
				echo "$env.BUILD_ID" - $env.BUILD_ID"
				echo "$env.JOB_NAME" - $env.JOB_NAME"
				echo "$env.BUILD_TAG" - $env.BUILD_TAG"
				echo "$env.BUILD_URL" - $env.BUILD_URL"
			}	
		}
		stage('Test') {
			steps {
				echo "Test"
			}	
		}
		stage('Integration Test') {
			steps {
				echo "Integration test"
			}	
		}
	}	
	post {
			always {
				echo 'I am awesome. I always run'
			}
			success {
				echo 'I run when you are successful'
			}
			failure {
				echo 'I run when you fail'
			}
			//changed
	}
}