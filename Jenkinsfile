library 'libAG'
pipeline {
    agent none
    stages {
        stage('Hello') {
            agent {label 'agent'}
            steps {
                pipelineMaven(['skipTest':false, 'skipInstall':true])
            }
        }
    }
}