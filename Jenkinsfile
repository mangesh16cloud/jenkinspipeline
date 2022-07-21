pipeline {
    agent any

    stages {
        stage('checkout') {
	    agent {
		lable 'Built-In Node'
	    }
            steps {
                echo 'Hello World'
		git url: "https://github.com/mangesh16cloud/jenkinspipeline.git"
		stash 'source'
            }
        }
        stage('1st-agent') {
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
