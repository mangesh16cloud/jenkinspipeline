node {
    stage('build') {
        sh 'java -version'
        echo 'this is build from SCM'
    }
    stage('test') {
	node('1st-agent'){
        sh 'w'
        echo 'this is test stage'
	}
    }
	    
    stage('deployment') {
        echo 'this is 1st deployment'
        echo 'this is deployment stage'
    }
}
