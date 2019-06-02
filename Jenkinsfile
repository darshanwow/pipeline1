pipeline {
	agent any;
	stages {
		stage('setup') {
			steps{
				cleanWs();
				sh 'echo setting up'
			}
		}
		stage('Checkout SCM') {
			steps{
				checkout scm
			}
		}
		stage('Compile') {
			steps{
				sh 'chmod a+x app.sh'
			}
		}
		stage('testing') {
			steps{
				sh 'sh app.sh'
			}
		}
	}
}

