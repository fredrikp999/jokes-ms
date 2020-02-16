node {
    checkout scm

    def customImage = docker.build("skonk/jokes-ms:${env.BUILD_ID}")

    customImage.inside {
        sh 'make test'
    }
}