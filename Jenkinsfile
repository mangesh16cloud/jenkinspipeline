node('1st-agent') {
    stage('build') {
        sh 'java -version'
        echo 'this is build from SCM'
        sh 'cp index.html'
    }
    stage('test') {
        sh 'w'
        echo 'this is test stage'
    }
    stage('deployment') {
        echo 'this is 1st deployment'
        echo 'this is deployment stage'
    }
}
