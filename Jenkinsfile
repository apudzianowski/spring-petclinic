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

                echo '\033[34mPipeline\033[0m \033[33mis\033[0m \033[35mstarting!\033[0m'
                pipelineMaven(['skipTest':false, 'skipInstall':true])
            }
        }
    }
}