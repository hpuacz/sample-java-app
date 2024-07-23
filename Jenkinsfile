node {
    properties(
    [
        pipelineTriggers([cron('17 30 * * *')]),
    ]
)
    /* Requires the Docker Pipeline plugin to be installed */
    docker.image('node:20.15.1-alpine3.20').inside {
        stage('Test') {
            sh 'node --version'
        }
    }
}
