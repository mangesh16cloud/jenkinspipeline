pipeline {
  agent any
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
	
        stage('build') {
	    
            steps {
		unstash 'source'
                echo 'Hello World'
            }
        }
    }
}
