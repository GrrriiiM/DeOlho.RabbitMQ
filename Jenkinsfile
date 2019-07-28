def exec(cmd) {
    if (Boolean.valueOf(env.UNIX)) {
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