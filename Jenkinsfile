node(){
    docker.image('node:lts-bullseye-slim').inside {
        stage('Build') {
            sh 'npm install'
        }
        stage('Test') {
            sh './jenkins/scripts/test.sh'
        }
    }
}