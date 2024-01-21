pipeline {
    agent any
    options {
     timestamps()
    }
    environment {
       K8s_NS = 'default'
       K8S_CREDS = 'kubernets-creds-faree'
    }
    stages {
        stage('Hello') {
            steps {
               echo "Your Executing ${BUILD_NUMBER}th build"
               sh './hello-world.sh'
            }
        }
