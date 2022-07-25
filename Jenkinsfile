pipeline {
    agent {'slave'}

    stages {
        stage('checkout') {
	    
            steps {
                echo 'Hello World'
		git url: "https://github.com/mangesh16cloud/jenkinspipeline.git"
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
