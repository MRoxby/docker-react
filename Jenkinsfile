pipeline {
    agent { 
        dockerfile {
             filename 'Dockerfile.dev'
             label 'MRoxby/docker-react'
             additionalBuildArgs '.'
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