pipeline {
    agent any

    stages {
		stage('Build') {
			steps {
				bat 'docker build -t "tp_note" .'
			}
		}
		stage('Run') {
			steps {
				bat 'docker run -p 127.0.0.1:3000:3000/tcp tp_note'
			}
		}
    }
}