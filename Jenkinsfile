pipeline {
    agent any

    stages {
        stage('checkout') {
	    agent {
		lable 'master'
	    }
            steps {
                echo 'Hello World'
		git url: "https://github.com/mangesh16cloud/jenkinspipeline.git"
		stash 'source'
            }
        }
        stage('build') {
	    agent {
		lable 'sonar-python'
	    }
            steps {
		unstash 'source'
                echo 'Hello World'
            }
        }
    }
}
