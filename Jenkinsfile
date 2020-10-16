@Library('github.com/Jim-Dawson-EMR/libraryTest') _

pipeline {
    agent any

    stages {
        stage('call lib') {
            steps {
                echo "$GIT_BRANCH"
                script{
                    helloWorld()
                }
            }
        }
        stage("libary function with arg") {
            steps {
                script {
                    helloArgs.("Jenkins!")
                }
            }            
        }
        stage("addl libary function with arg") {
            steps {
                script {
                    helloArgs.goodbyeWorld("Jenkins!")
                }
            }            
        }
    }
}
