node {
    stage('build') {
        sh 'java -version'
        echo 'this is build from SCM'
    }
    stage('test') {
        sh 'w'
        echo 'this is test stage'
    }
    stage('deployment') {
        withSonarQubeEnv ('sonarqube-8.9'){
         echo 'this is deploy stage' 
        echo 'this is 1st deployment'
        echo 'this is deployment stage'
        }
    }
}
