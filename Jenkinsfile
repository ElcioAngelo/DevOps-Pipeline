pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                script {
		sh '''
		docker stop $(docker ps -aq) && docker rm $(docker ps -aq)
		docker compose up --build 
		docker compose up -d 	
	        '''  
		}
            }
        }
    }
}
