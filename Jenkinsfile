node {
    stage('Checkout'){
        checkout scm
    }

    stage ('Build Image'){
        def customImage = docker.build("skonk/jokes-ms:${env.BUILD_ID}")
    }
}