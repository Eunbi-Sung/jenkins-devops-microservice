pipeline {
	agent any
	// agent { docker { image "maven:3.6.3" } }
	// agent { docker { image "node:13.8" } }
	stages {
		stage('Build') {
			steps {
				// sh "mvn --version"
				// sh "node --version"
				echo "Build"
				echo "PATH - $PATH"
				echo "BUILD_NUMBER - $env.BUILD_NUMBER"
				echo "BUILD_ID - $euv.BUILD_ID"
				echo "JOB_NAME - $euv.JOB_NAME"
				echo "BUILD_TAG - $euv.BUILD_TAG"
				echo "BUILD_URL - $euv.BUILD_URL"
			}
		}
				stage('Test') {
			steps {
				echo "Test"
			}
		}
				stage('Deploy') {
			steps {
				echo "Deploy"
			}
		}
	}

	post {
		always {
			echo "I run always"
		}
		success {
			echo "I run when you are successful"
		}
		failure {
			echo "I run when you fail"
		}
	}
}
