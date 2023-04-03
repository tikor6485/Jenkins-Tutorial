pipeline {
    agent {label "Linux"}
    options {
        buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '')
        disableConcurrentBuilds()
    }
    stages {
        stage ('Hello') {
            steps {
                echo 'hello'
            }
        }
        stage ('cat README') {
            when {
                branch "fix-*"
            }
            steps {
                sh '''
                    cat README.md
                '''
            }
        }
    }
}
