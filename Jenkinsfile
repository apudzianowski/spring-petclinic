library 'libAG'
pipeline {
    agent none
    options {
        ansiColor('xterm')
    }
    stages {
        stage('Hello') {
            agent {label 'agent'}
            steps {
                echo '\033[35mPipeline\033[0m \033[35mis\033[0m \033[35mstarting!\033[0m'
                pipelineMaven(['skipTest':true, 'skipInstall':true])
            }
        }
    }
}