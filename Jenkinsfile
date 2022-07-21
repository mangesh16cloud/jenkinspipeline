pipeline {
    agent '1st-agent'

    stages {
        stage('checkout') {
	    agent {
		lable '1st-agent'
	    }
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
