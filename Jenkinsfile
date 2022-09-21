node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub') {

        def customImage = docker.build("005907/jenkins-docker-test")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
