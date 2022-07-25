pipeline {
    agent {
  label {
    label 'slave'
    retries 2
  }

    stages {
        stage('checkout') {
	    
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
