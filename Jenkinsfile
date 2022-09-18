node(){
    withDockerContainer(args: '-p 3000:3000', image: 'node:lts-bullseye-slim') {
    stage('Build') {
            sh 'npm install'
        }
        stage('Test') {
            sh './jenkins/scripts/test.sh'
        }
    }
}