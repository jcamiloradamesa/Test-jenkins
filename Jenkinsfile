node {
    stage("Run") {

        def projectX =  checkout([$class: 'GitSCM',
            branches: [[name: 'origin/master']],
            extensions: [[$class: 'WipeWorkspace']],
            userRemoteConfigs: [[credentialsId: 'GH-RO', url: 'https://github.com/jcamiloradamesa/Test-jenkins']]
        ])

        env.GIT_PREVIOUS_COMMIT = projectX.GIT_PREVIOUS_COMMIT
        env.GIT_COMMIT = projectX.GIT_COMMIT
        println "from:${env.GIT_PREVIOUS_COMMIT} - to: ${env.GIT_COMMIT}"
    }
}