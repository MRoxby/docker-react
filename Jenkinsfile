pipeline {
    agent { 
        docker {
             filename 'Dockerfile.dev'
             label 'MRoxby/docker-react'
             dir '.'
              } 
            }
    stages {
        stage('build') {
            steps {
                sh 'docker run MRoxby/docker-react npm run test -- --coverage'
            }
        }
    }
}