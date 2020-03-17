node ('master'){
    stage ('docker build'){
    bat 'docker build -t mroxby/docker-react -f dockerfile.dev .'
    bat 'docker run mroxby/docker-react npm run test -- --coverage'
    }
}