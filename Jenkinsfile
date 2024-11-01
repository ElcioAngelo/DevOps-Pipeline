pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                // 
            }
        }
        stage('Deploy') { 
            steps {
                sh '''
			sudo docker compose up --build 
		''' 
            }
        }
    }
}
