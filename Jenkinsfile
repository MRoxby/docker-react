node ('master'){
    stage ('docker build'){
    bat 'docker build -t mroxby/docker-react -f dockerfile.dev .'
    bat 'docker run -p 3000:3000 mroxby/docker-react'
    }
}