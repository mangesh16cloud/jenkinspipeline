pipeline {
  agent any
	environment{
		DOCKER_TAG = getDockerTag()
	}
	
    stages {
        stage('checkout') {
	     agent { 
    		label 'slave'
		}
            steps {
		git branch: 'main', url: 'https://github.com/mangesh16cloud/jenkinspipeline.git'
		stash 'source'
            }
        }
	
        stage('build with DOCKER IMG') {
	    
            steps {
		unstash 'source'
		sh "docker build . -t mangeshsk/test:${DOCKER_TAG}"
                echo 'Hello World'
            }
        }
    }
}
