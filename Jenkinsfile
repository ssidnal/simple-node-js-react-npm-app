pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'cd /var/jenkins_home/workspace/simple-node-js-react-npm-app && npm install' 
            }
        }
    }
}