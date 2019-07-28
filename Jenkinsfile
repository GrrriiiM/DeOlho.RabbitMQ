def exec(cmd) {
    if (isUnix()) {
        sh cmd
    }
    else {
        bat cmd
    }
}

node {
    stage('Docker-compose up') {
        exec('docker-compose up -d')
    }
}