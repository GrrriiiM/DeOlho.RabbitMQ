def exec(cmd) {
    if (isUnix()) {
        sh cmd
    }
    else {
        bat cmd
    }
}

node {
    stage('Git pull') {
        checkout scm
    }
    stage('Docker-compose up') {
        exec('docker-compose up -d')
    }
}