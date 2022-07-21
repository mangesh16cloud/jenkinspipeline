pipeline {
    agent any

    stages {
        stage('checkout') {
	    agent {
		lable ('any')
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
