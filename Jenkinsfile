pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                //
		sh '''
			sudo mkdir DevOps-Pipeline 
			cd DevOps-Pipeline
                        git clone https://github.com/ElcioAngelo/DevOps-Pipeline.git
			sudo docker compose up --build
				
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
