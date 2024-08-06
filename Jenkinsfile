pipeline {
    agent {
        docker{
            image'node:16-buster-slim'
        }
    }
    stages {
    stage('Build'){
        steps{
            sh 'npm install'
        }
    }


    stages('Test'){
        steps {
            sh './jenkins/scripts/test.sh'
            }
        }
    }
}