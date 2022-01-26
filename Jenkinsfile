pipeline {
    agent any
		stage('Run') {
			steps {
				bat 'docker build -t "tp_note" .'
				bat 'docker run -p 0.0.0.0:3000:3000/tcp tp_note'
			}
		}
}