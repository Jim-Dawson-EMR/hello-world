@Library('github.com/Jim-Dawson-EMR/libraryTest') _

pipeline {
    agent any

    stages {
        stage('show branch') {
            steps {
                echo "$GIT_BRANCH"
            }
        }
        stage("libary function no arg") {
            steps {
                script {
                    helloWorld()
                }
            }            
        }
/*        stage("libary function with arg") {
            steps {
                script {
                    helloArgs.('Jenkins!')
                }
            }            
        }*/
        stage("addl libary function with arg") {
            steps {
                script {
                    helloArgs.goodbyeWorld('Jenkins!')
                }
            }            
        }
    }
}
