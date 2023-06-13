library 'libAG'
pipeline {
    agent any
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
    post {
        always{
        echo '\033[33mCzyszcze\033[0m \033[33mci\033[0m \033[33mrure!\033[0m'
        cleanWs()
    }
}
}