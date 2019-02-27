node {
    stage("Run") {
        sh "echo from:${System.getenv('GIT_PREVIOUS_SUCCESSFUL_COMMIT')} - to: ${System.getenv('GIT_COMMIT')}"
    }
}