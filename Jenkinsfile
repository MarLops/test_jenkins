pipeline {
    agent {
        docker { image 'hello-world' }
    }
    stages {
         stage('Initialize'){
            def dockerHome = tool 'myDocker'
            env.PATH = "${dockerHome}/bin:${env.PATH}"
         }
        stage('Build') {
            steps {
                echo 'Helo'
            }
        }
    }
}
