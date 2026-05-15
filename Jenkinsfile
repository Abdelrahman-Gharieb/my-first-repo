pipeline {
	agent any
	environment {
		GREETING = "Hello from Jenkins Pipeline!"
	}
	stages {
		stage('Build') {
			steps {
				echo 'Building project...'
				echo "$GREETING"
			}
		}
		stage('Test') {
			steps {
				echo 'Running tests...'
				echo 'Tests Passed!'
			}
		}
		stage('Deploy') {
			steps {
				echo 'Deploying application...'
			}
		}
	}
	post {
		success {
			echo 'Pipeline completed successfully!'
		}
		failure {
			echo 'Pipeline failed!'
		}
	}
}