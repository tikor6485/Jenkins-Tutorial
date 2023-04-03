pipeline {
    agent {lable "Linux"}
    options {
        buildDiscarder logRotator(artifactDaysTokeepStr: '', artifactNumToKeepS>
        disableConcrrentBuilds()
    }
    stages {
        stage ('Hello'){
            steps{
                echo 'hello'
            }
        }
        stage ('cat README'){
            when {
                branch "fix-*"
            }
            steps{
               sh '''
                cat README.md
            }
        }
    }

}
