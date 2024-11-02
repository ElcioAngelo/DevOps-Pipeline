pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                //
		sh '''
		cd DevOps-Pipeline
		 docker compose up --build
				
	           '''  
            }
        }
        stage('Deploy') { 
            steps {
		sh '''
			docker compose up -d 
		'''
            }
        }
    }
}
