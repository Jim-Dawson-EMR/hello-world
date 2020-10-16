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
    }
}
