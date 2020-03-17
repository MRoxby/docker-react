pipeline {
    agent { 
        docker {
             filename 'Dockerfile.dev'
             label 'mroxby/docker-react'
             dir '.'
              } 
            }
    stages {
        stage('test') {
            steps {
                sh 'docker run mroxby/docker-react npm run test -- --coverage'
            }
        }
    }
}