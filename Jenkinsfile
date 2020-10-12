node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'docker_credential_it') {

        def customImage = docker.build("rpuran/practice:21.1")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
