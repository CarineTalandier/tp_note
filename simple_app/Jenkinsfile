pipeline {
    agent any

    stages {
       stage('Pull') {
			steps {
				git([url:'https://github.com/CarineTalandier/tp_note', branch:'master'])
			}
		}
		stage('Build') {
			steps {
				bat 'docker build -t "tp_note" .'
				bat 'docker run -p 0.0.0.0:3000:3000/tcp tp_note'
			}
		}
    }
}