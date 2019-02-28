node {
    stage("Init") {
            steps {
                script {
                    deleteDir()
                    checkout scm
                }
            }
    }

    stage("Run") {
        sh "./run.sh"
    }
}