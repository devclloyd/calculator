pipeline {
	agent any
		stages {
			stage('Checkout') {
				steps {
					git url: 'https://github.com/clloyd12/calculator.git'
				}
			}
			stage('Compile') {
				steps {
					sh "./gradlew compileJava"
				}
			}
			stage('Unit Test') {
				steps {
					sh "./gradlew test"
				}
			}
		}
}
