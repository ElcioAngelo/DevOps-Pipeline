pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                //
		sh '''
		 mkdir DevOps-Pipeline 
		cd DevOps-Pipeline
                git clone https://github.com/ElcioAngelo/DevOps-Pipeline.git
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
