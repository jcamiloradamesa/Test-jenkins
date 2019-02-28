node {
    stage("Run") {

        def projectX =  checkout scm

        env.GIT_PREVIOUS_COMMIT = projectX.GIT_PREVIOUS_COMMIT
        env.GIT_COMMIT = projectX.GIT_COMMIT
        env.GIT_PREVIOUS_SUCCESSFUL_COMMIT = projectX.GIT_PREVIOUS_SUCCESSFUL_COMMIT
        println "from:${env.GIT_PREVIOUS_COMMIT} - to: ${env.GIT_COMMIT} and ${env.GIT_PREVIOUS_SUCCESSFUL_COMMIT}"
    }
}