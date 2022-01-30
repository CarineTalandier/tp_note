pipeline {
    agent any

    stages {
       
		stage('Build') {
			steps {
				bat 'cd  ~/Documents/Efrei/DataEngineering/tp_jenkins_docker_note/tp_note'
				bat 'docker build -t "tp_note" .'
				bat 'docker run -p 0.0.0.0:3000:3000/tcp tp_note'
			}
		}
    }
}