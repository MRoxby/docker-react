node ('master'){
    stage('git'){
        git 'clone https://github.com/MRoxby/docker-react.git'
    }
    stage ('docker build'){
    bat 'docker build -t mroxby/docker-react -f dockerfile.dev .'
    bat 'docker run -p 3000:3000 mroxby/docker-react'
   //bat 'docker run mroxby/docker-react npm run test -- --coverage'
    }
    stage ('deploy'){
        
    }
}