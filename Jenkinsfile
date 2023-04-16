pipeline {
    agent any // use any available agent to run this pipeline
    stages { // define the stages of this pipeline
        stage('Build') { // define a stage called "Build"
            steps { // define the steps of this stage
                sh 'rm -rf Jenkins_Tutorial'
                sh 'git clone https://github.com/tikor6485/Jenkins_Tutorial.git'
                sh 'mvn clean -f Jenkins_Tutorial'
            }
        }
        stage('Test') { // define a stage called "Test"
            steps { // define the steps of this stage
                sh 'mvn test -f Jenkins_Tutorial'
            }
        }
        stage('Deploy') { // define a stage called "Deploy"
            steps { // define the steps of this stage
                sh 'mvn package -f Jenkins_Tutorial'
            }
        }
    }
}
