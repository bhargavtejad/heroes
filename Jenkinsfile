pipeline {
	agent any

	tools {nodejs "node"}

	stages {

		stage('Cloning Git') {

			steps {
				git 'https://github.com/bhargavtejad/heroes.git'
			}
		}

		stage('Install Dependencies') {

			steps {
				bat 'npm install'
			}
		}

		stage('Test') {

			steps {
				bat 'npm test'
			}
		}
	}
}