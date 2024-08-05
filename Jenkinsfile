pipeline {
	agent { docker { image "maven:3.6.3" } }
	stages {
		stage('Build') {
			steps {
				sh "mvn --version"
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
