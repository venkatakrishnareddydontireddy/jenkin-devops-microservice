// Declarative pipeline

pipeline {
		//agent any
		agent { docker { image 'node:13.8' } }
		stages {
			stage('Build') {
				steps {
					sh 'node --version'
					echo "Build"
				}
			}
			stage('Test') {
				steps {
					echo "Test"
				}
			}
			stage('Integration Testing') {
				steps {
					echo "Integration Testing"
				}
			}
		}
		post {
			always {
				echo " Im awesome. I run always"
			}
			success {
				echo " I run when you are successful"
			}
			failure {
				echo " I run when you fail"
			}
			changed {
				echo " I run when you changed"
			}
			unstable {
				echo " I run when you unstable"
			}
		}
}
